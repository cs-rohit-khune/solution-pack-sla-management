# What's New

<table>
    <tr>
        <th>Compatible Version</th>
        <td>FortiSOAR v7.6.0 and later</td>
    </tr>
</table>

- Properly calculates **Response Due Date** and **Response SLA** when status changes (e.g., Open → Investigating → Pending → Investigating).  
- Correctly sets **Acknowledge Due Date** if an alert moves from **Open → Closed**.  
- Ensures accurate **Ack Due Date** and **Ack Date** when an alert is updated to **Investigating** immediately after creation.