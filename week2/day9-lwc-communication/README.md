# Day 9 - LWC Communication

## Component Communication
- Child to Parent Communication
- Parent to Child Communication
- Lightning Message Service (LMS)

## Dashboard Design
- Left Region → Numerator + Controls
- Center Region → Augmentor + Numerator
- Right Region → RemoteControl + Counts

## Data Flow Explanation
- Controls → Numerator
- Augmentor → Numerator
- RemoteControl → Message Channel → Counts

## Aura vs LWC

| Aura | LWC |
|---|---|
| Proprietary | Web Standards |
| Slower | Faster |
| Complex | Simpler |
| Aura Events | DOM Events |

## Reflection
This project helped in understanding:
- Component communication
- LMS
- Modular architecture
- Enterprise UI design

## Revision Questions

1. Why do components communicate?  
To share data and trigger actions.

2. Difference between parent-child communication and events?  
Parent-child uses properties/methods, events notify parents.

3. Why is modular architecture useful?  
Improves reusability and maintainability.

4. Why did Salesforce move toward LWC?  
Better performance and web standards support.

5. What problems happen in tightly coupled systems?  
Difficult maintenance and scalability issues.

6. Why is frontend architecture important?  
Improves organization and user experience.

7. Why should UI and backend remain separate?  
For scalability and maintainability.

8. Why do large systems need reusable modules?  
To reduce development time and improve consistency.

## End of Day Outcome
- Component communication
- Modern UI architecture
- Data flow in applications
- Modular enterprise system design
- Importance of LWC

