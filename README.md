# 5gr-pilots
Repo to upload the descriptors of the different use cases/pilots


# Experiment Catalogue

To support reproducibility/comparison efforts, we provide hereunder a Service KPI index of the experiments conducted in Work Package 4, aiming to capture the different ways a given SKPI has been measured. For each SKPI, we list all pilot use-cases evaluating them, the corresponding Core KPIs, and summarize key informations on the used tools. Note that the detailed measurement procedures for each pilot/use-case are available in deliverable [D4.2](https://5growth.eu/wp-content/uploads/2019/06/D4.2-Verification_methodology_and_tool_design.pdf), with minor updates in [D4.3](https://5growth.eu/wp-content/uploads/2019/06/D4.3-5G_facility_validation_and_verification_report.pdf) and [D4.4](https://5growth.eu/deliverables/).

>**Index**
>
>  1. [Service Setup Time (5GR-SKPI-1)](#service-setup-time-5gr-skpi-1)
>  1. [Synchronization between communication components (5GR-SKPI-2)](#synchronization-between-communication-components-5gr-skpi-2)
>  1. [Device Mobility (5GR-SKPI-3)](#device-mobility-5gr-skpi-3)
>  1. [High-resolution Real-time Video Quality (5GR-SKPI-4)](#high-resolution-real-time-video-quality--5gr-skpi-4)
>  1. [Radius of Operation (5GR-SKPI-5)](#radius-of-operation-5gr-skpi-5)
>  1. [Integrated Multitype Communications (5GR-SKPI-6)](#integrated-multitype-communications-5gr-skpi-6)
>  1. [Extensive Network Coverage in Vertical Premises (5GR-SKPI-7)](#extensive-network-coverage-in-vertical-premises-5gr-skpi-7)
>  1. [Service Operation Time (5GR-SKPI-8)](#service-operation-time-5gr-skpi-8)
>  1. [Service Operation Capacity (5GR-SKPI-9)](#service-operation-capacity-5gr-skpi-9)
>  1. [Service Availability (5GR-SKPI-10)](#service-availability-5gr-skpi-10)
>  1. [Service Reaction Time (5GR-SKPI-11)](#service-reaction-time-5gr-skpi-11)


## Service Setup Time (5GR-SKPI-1)

<table>
    <thead>
        <tr>
            <th>Pilot</th>
            <th>Use-Cases</th>
            <th>Measured CKPIs</th>
            <th>Tools</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td rowspan=2>INNOVALIA</td>
            <td rowspan=2>UC1, UC2</td>
            <td>CKPI-5 Availability</td>
            <td>See D4.3 Section 3.1.1<br/>Assumed to be >99.999%</td>
        </tr>
        <tr>
            <td>CKPI-6 Slice creation time</td>
            <td>Vertical Slicer log analyzis</td>
        </tr>
    </tbody>
</table>

## Synchronization between communication components (5GR-SKPI-2)

<table>
    <thead>
        <tr>
            <th>Pilot</th>
            <th>Use-Cases</th>
            <th>Measured CKPIs</th>
            <th>Tools</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td rowspan=2>INNOVALIA</td>
            <td rowspan=2>UC1, UC2</td>
            <td>CKPI-1 End-to-End Latency</td>
            <td>Pings, Application-experienced RTT, TCP srtt. Measured using 5Probe</td>
        </tr>
        <tr>
            <td>CKPI-2 Packet loss</td>
            <td>See D4.3 Section 3.1.1<br/>Assumed to be <2%</td>
        </tr>
        <tr>
            <td rowspan=2>COMAU</td>
            <td rowspan=2>UC1</td>
            <td>CKPI-1 End-to-End Latency</td>
            <td>LaTe</td>
        </tr>
        <tr>
            <td>CKPI-2 Packet loss</td>
            <td>LaTe</td>
        </tr>
        <tr>
            <td rowspan=4>EFFACEC_S</td>
            <td rowspan=2>UC1</td>
            <td>CKPI-1 End-to-End Latency</td>
            <td>ping</td>
        </tr>
        <tr>
            <td>CKPI-2 Packet loss</td>
            <td>ping<br/>Train detector application and/or simulator</td>
        </tr>
        <tr>
            <td rowspan=2>UC2</td>
            <td>CKPI-1 End-to-End Latency</td>
            <td>Ping every 0.2s, during >15mins, using UDP packets of 1KB</td>
        </tr>
        <tr>
            <td>CKPI-2 Packet loss</td>
            <td>iperf3</td>
        </tr>
        <tr>
            <td rowspan=2>EFFACEC_E</td>
            <td rowspan=2>UC1</td>
            <td>CKPI-1 End-to-End Latency</td>
            <td>ping</td>
        </tr>
        <tr>
            <td>CKPI-2 Packet loss</td>
            <td>iperf</td>
        </tr>
    </tbody>
</table>

## Device Mobility (5GR-SKPI-3)

<table>
    <thead>
        <tr>
            <th>Pilot</th>
            <th>Use-Cases</th>
            <th>Measured CKPIs</th>
            <th>Tools</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>INNOVALIA</td>
            <td>UC2</td>
            <td>CKPI-3 Guaranteed data rate</td>
            <td>5Probe (passive throughput measurement)</td>
        </tr>
        <tr>            
            <td rowspan=3>COMAU</td>
            <td rowspan=3>UC3</td>
            <td>CKPI-3 Guaranteed data rate</td>
            <td>iperf2</td>
        </tr>
        <tr>
            <td>CKPI-10 Received Radio Signal Quality</td>
            <td>Assumed perfect due to experimental conditions</td>
        </tr>
        <tr>
            <td>CKPI-11 Buffer Occupancy</td>
            <td>Smooth application playback</td>
        </tr>
    </tbody>
</table>

## High-resolution Real-time Video Quality  (5GR-SKPI-4)

<table>
    <thead>
        <tr>
            <th>Pilot</th>
            <th>Use-Cases</th>
            <th>Measured CKPIs</th>
            <th>Tools</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td rowspan=2>INNOVALIA</td>
            <td rowspan=2>UC1</td>
            <td>CKPI-3 Guaranteed data rate</td>
            <td>5Probe (passive throughput measurement)</td>
        </tr>
        <tr>
            <td>CKPI-9 Jitter</td>
            <td>Derived from ping inter-arrivals</td>
        </tr>
        <tr>
            <td rowspan=3>COMAU</td>
            <td rowspan=3>UC3</td>
            <td>CKPI-2 Packet loss</td>
            <td>LaTe</td>
        </tr>
        <tr>
            <td>CKPI-3 Guaranteed data rate</td>
            <td>iperf2</td>
        </tr>
            <tr>
            <td>CKPI-9 Jitter</td>
            <td>LaTe</td>
        </tr>
        <tr>
            <td rowspan=3>EFFACEC_S</td>
            <td rowspan=3>UC2</td>
            <td>CKPI-2 Packet loss</td>
            <td>ping</td>
        </tr>
        <tr>
            <td>CKPI-3 Guaranteed data rate</td>
            <td>iperf</td>
        </tr>
            <tr>
            <td>CKPI-9 Jitter</td>
            <td>ping</td>
        </tr>
        <tr>
            <td rowspan=2>EFFACEC_E</td>
            <td rowspan=2>UC1</td>
            <td>CKPI-2 Packet loss</td>
            <td>ping</td>
        </tr>
        <tr>
            <td>CKPI-9 Jitter</td>
            <td>ping</td>
        </tr>
    </tbody>
</table>

## Radius of Operation (5GR-SKPI-5)

<table>
    <thead>
        <tr>
            <th>Pilot</th>
            <th>Use-Cases</th>
            <th>Measured CKPIs</th>
            <th>Tools</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td rowspan=2>INNOVALIA</td>
            <td rowspan=2>UC1</td>
            <td>CKPI-1 End-to-End Latency</td>
            <td>Pings, Application-experienced RTT, TCP srtt. Measured using 5Probe</td>
        </tr>
        <tr>
            <td>CKPI-5 Availability</td>
            <td>See D4.3 Section 3.1.1<br/>Assumed to be >99.999%</td>
        </tr>
    </tbody>
</table>

## Integrated Multitype Communications (5GR-SKPI-6)

<table>
    <thead>
        <tr>
            <th>Pilot</th>
            <th>Use-Cases</th>
            <th>Measured CKPIs</th>
            <th>Tools</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td rowspan=2>INNOVALIA</td>
            <td rowspan=2>UC1</td>
            <td>CKPI-1 End-to-End Latency</td>
            <td>Pings, Application-experienced RTT, TCP srtt. Measured using 5Probe</td>
        <tr>
            <td>CKPI-3 Guaranteed data rate</td>
            <td>5Probe (passive throughput measurement)</td>
        </tr>
    </tbody>
</table>

## Extensive Network Coverage in Vertical Premises (5GR-SKPI-7)

<table>
    <thead>
        <tr>
            <th>Pilot</th>
            <th>Use-Cases</th>
            <th>Measured CKPIs</th>
            <th>Tools</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td rowspan=5>INNOVALIA</td>
            <td rowspan=5>UC1, UC2</td>
            <td>CKPI-1 End-to-End Latency</td>
            <td>Pings, Application-experienced RTT, TCP srtt. Measured using 5Probe</td>
        <tr>
            <td>CKPI-2 Packet loss</td>
            <td>See D4.3 Section 3.1.1<br/>Assumed to be <2%</td>
        </tr>
        <tr>
            <td>CKPI-3 Guaranteed data rate</td>
            <td>5Probe (passive throughput measurement)</td>
        </tr>
        <tr>
            <td>CKPI-5 Availability</td>
            <td>See D4.3 Section 3.1.1<br/>Assumed to be >99.999%</td>
        </tr>
       <tr>
            <td>CKPI-7 Connection density</td>
            <td>Not measured see D4.3 Section 3.1.1. Not supported by the 5G EVE platform</td>
        </tr>
        <tr>
            <td rowspan=5>COMAU</td>
            <td rowspan=5>UC1, UC2</td>
            <td>CKPI-1 End-to-End Latency</td>
            <td>LaTe</td>
        <tr>
            <td>CKPI-2 Packet loss</td>
            <td>LaTe</td>
        </tr>
        <tr>
            <td>CKPI-3 Guaranteed data rate</td>
            <td>iperf</td>
        </tr>
        <tr>
            <td>CKPI-5 Availability</td>
            <td>See D4.3 Section 3.2.1. Not measured</td>
        </tr>
       <tr>
            <td>CKPI-7 Connection density</td>
            <td>Emulated through analytical models</td>
        </tr>
    </tbody>
</table>

## Service Operation Time (5GR-SKPI-8)

<table>
    <thead>
        <tr>
            <th>Pilot</th>
            <th>Use-Cases</th>
            <th>Measured CKPIs</th>
            <th>Tools</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td rowspan=2>INNOVALIA</td>
            <td rowspan=2>UC2</td>
            <td>CKPI-1 End-to-End Latency</td>
            <td>Pings, Application-experienced RTT, TCP srtt. Measured using 5Probe</td>
        <tr>
            <td>CKPI-3 Guaranteed data rate</td>
            <td>5Probe (passive throughput measurement)</td>
        </tr>
    </tbody>
</table>

## Service Operation Capacity (5GR-SKPI-9)

<table>
    <thead>
        <tr>
            <th>Pilot</th>
            <th>Use-Cases</th>
            <th>Measured CKPIs</th>
            <th>Tools</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td rowspan=2>INNOVALIA</td>
            <td rowspan=2>UC2</td>
            <td>CKPI-3 Guaranteed data rate</td>
            <td>5Probe (passive throughput measurement)</td>
        </tr>
        <tr>
            <td>CKPI-5 Availability</td>
            <td>See D4.3 Section 3.1.1<br/>Assumed to be >99.999%</td>
        </tr>
    </tbody>
</table>

## Service Availability (5GR-SKPI-10)

<table>
    <thead>
        <tr>
            <th>Pilot</th>
            <th>Use-Cases</th>
            <th>Measured CKPIs</th>
            <th>Tools</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>EFFACEC_S</td>
            <td>UC1, UC2</td>
            <td>CKPI-5 Availability</td>
            <td>Uptime (radio + QoS + services) over one month</td>
        <tr>
            <td>EFFACEC_E</td>
            <td>UC1, UC2</td>
            <td>CKPI-5 Availability</td>
            <td>Uptime (radio + QoS + services) over one month</td>
        </tr>
    </tbody>
</table>

## Service Reaction Time (5GR-SKPI-11)

Not measured in any pilot UC.

-------------------

### Project information
5GROWTH is funded by the European Union’s Research and Innovation Programme Horizon 2020 under Grant Agreement no. 856709


Call: H2020-ICT-2019. Topic: ICT-19-2019. Type of action: RIA. Duration: 30 Months. Start date: 1/6/2019


<p align="center">
<img src="https://upload.wikimedia.org/wikipedia/commons/b/b7/Flag_of_Europe.svg" width="100px" />
</p>

<p align="center">
<img src="https://5g-ppp.eu/wp-content/uploads/2019/06/5Growth_rgb_horizontal.png" width="300px" />
</p>
 


