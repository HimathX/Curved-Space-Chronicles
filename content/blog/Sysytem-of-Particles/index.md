---
title: 🌍 System of Particles
summary: Linear momentum of a particle system stays constant if no external force acts. In the center of mass frame, total momentum is zero. Angular momentum changes due to external torque and can also be considered about the center of mass.
date: 2025-04-13
math: true

image:
  caption: 'Image credit: [**MS Designer**](https://designer.microsoft.com/)'

authors:
  - admin
  - HimathX

tags:
  - Particles
---

## Linear Momentum of a System

Linear momentum of a system of particles is defined as the sum of the momenta of individual particles:

{{< math >}}
$$
\vec{P}_{\text{sys}} = \sum_{j=1}^n \vec{P}_j
$$
{{< /math >}}

### Center of Mass
Position vector to the center of mass from an origin \( O \) is:

{{< math >}}
$$
\vec{R}_{\text{CM}} = \frac{\sum_{j=1}^n m_j \vec{r}_j}{\sum_{j=1}^n m_j}
$$
{{< /math >}}

Differentiating with respect to time:

{{< math >}}
$$
M \vec{V}_{\text{CM}} = \sum_{j=1}^n m_j \vec{v}_j = \vec{P}_{\text{sys}} \Rightarrow \vec{P}_{\text{sys}} = M \vec{V}_{\text{CM}}
$$
{{< /math >}}

Differentiating again:

{{< math >}}
$$
M \vec{a}_{\text{CM}} = \sum_{j=1}^n m_j \vec{a}_j
$$
{{< /math >}}

If the origin is inertial:

{{< math >}}
$$
m_j \vec{a}_j = \vec{F}_j
$$
{{< /math >}}

Where \( \vec{F}_j \) includes both external and internal forces:

{{< math >}}
$$
\vec{F}_j = \vec{F}_j^{\text{ext}} + \vec{F}_j^{\text{int}}, \quad \vec{F}_j^{\text{int}} = \sum_{i \neq j} \vec{F}_{j,i}
$$
{{< /math >}}

Substituting:

{{< math >}}
$$
M \vec{a}_{\text{CM}} = \sum_{j=1}^n \left( \vec{F}_j^{\text{ext}} + \sum_{i \neq j} \vec{F}_{j,i} \right) = \sum_{j=1}^n \vec{F}_j^{\text{ext}}
$$
{{< /math >}}

Thus:

{{< math >}}
$$
\vec{F}_{\text{ext}} = M \vec{a}_{\text{CM}} = \frac{d\vec{P}_{\text{sys}}}{dt}
$$
{{< /math >}}

### Conservation of Momentum
If \( \vec{F}_{\text{ext}} = 0 \), then:

{{< math >}}
$$
\frac{d\vec{P}_{\text{sys}}}{dt} = 0 \Rightarrow \vec{P}_{\text{sys}} = \text{constant}
$$
{{< /math >}}

### Linear Momentum in Center of Mass Frame
Let \( \vec{v'}_j = \vec{v}_{j,CM} = \vec{v}_{j,O} - \vec{v}_{CM,O} \), then:

{{< math >}}
$$
\vec{P}_{\text{sys,CM}} = \sum_{j=1}^n m_j \vec{v'}_j = 0
$$
{{< /math >}}

### Summary
- **Momentum:** \( \vec{P} = M \vec{v}_{\text{CM}} \)
- **Rate of change:** \( \vec{F}_{\text{ext}} = M \vec{a}_{\text{CM}} = \frac{d\vec{P}_{\text{sys}}}{dt} \)
- **Momentum is conserved if \( \vec{F}_{\text{ext}} = 0 \)**
- \( \vec{P}_{\text{sys,CM}} = 0 \)

## Angular Momentum of a System of Particles

### Angular Momentum about a Fixed Origin
Angular momentum:

{{< math >}}
$$
\vec{L}_{\text{sys}} = \sum_{j=1}^n \vec{r}_j \times \vec{p}_j
$$
{{< /math >}}

Differentiating:

{{< math >}}
$$
\frac{d\vec{L}_{\text{sys}}}{dt} = \sum_{j=1}^n \left( \vec{r}_j \times \frac{d\vec{p}_j}{dt} + \frac{d\vec{r}_j}{dt} \times \vec{p}_j \right) = \sum_{j=1}^n \vec{r}_j \times \vec{F}_j
$$
{{< /math >}}

As before:

{{< math >}}
$$
\frac{d\vec{L}_{\text{sys}}}{dt} = \sum_{j=1}^n \left( \vec{r}_j \times \vec{F}_j^{\text{ext}} + \frac{1}{2} \sum_{i \neq j} (\vec{r}_{j,i} \times \vec{F}_{j,i}) \right)
$$
{{< /math >}}

Since \( \vec{r}_{j,i} \) and \( \vec{F}_{j,i} \) are parallel:

{{< math >}}
$$
\vec{r}_{j,i} \times \vec{F}_{j,i} = 0 \Rightarrow \frac{d\vec{L}_{\text{sys}}}{dt} = \sum_{j=1}^n \vec{r}_j \times \vec{F}_j^{\text{ext}} = \vec{\tau}_{\text{ext}}
$$
{{< /math >}}

### Angular Momentum and COM
Let \( \vec{r}_j = \vec{R} + \vec{r'}_j \), \( \vec{v}_j = \vec{v}_{CM} + \vec{v'}_j \), then:

{{< math >}}
$$
\vec{L}_O = \sum_{j=1}^n (\vec{R} + \vec{r'}_j) \times m_j (\vec{v}_{CM} + \vec{v'}_j)
$$
{{< /math >}}

{{< math >}}
$$
= \vec{R} \times M \vec{v}_{CM} + \sum_{j=1}^n m_j \vec{r'}_j \times \vec{v'}_j = \vec{R} \times \vec{P}_{\text{sys}} + \vec{L}_{\text{CM}}
$$
{{< /math >}}

Differentiating:

{{< math >}}
$$
\frac{d\vec{L}_O}{dt} = \frac{d\vec{L}_{CM}}{dt} + \vec{R} \times \vec{F}_{\text{ext}}
$$
{{< /math >}}

Also:

{{< math >}}
$$
\vec{\tau}_O = \sum_{j=1}^n (\vec{r'}_j + \vec{R}) \times \vec{F}_j = \sum_{j=1}^n \vec{r'}_j \times \vec{F}_j + \vec{R} \times \sum_{j=1}^n \vec{F}_j
$$
{{< /math >}}


## Download Full Notes
[Download the complete PDF notes here](Physics_Notes.pdf)