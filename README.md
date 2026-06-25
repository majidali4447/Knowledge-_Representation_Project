# Cultural Heritage and Museum Ontology

## OWL 2 Implementation using Protégé

---

## 1. Knowledge Domain

This ontology belongs to the **Cultural Heritage and Museum Management Domain**.

It provides a semantic representation of cultural heritage resources, museum collections, artworks, artifacts, exhibitions, historical periods, conservation activities, materials, locations, and digital documentation resources.

The ontology is intended to support knowledge organization, semantic interoperability, and automated reasoning within museum and heritage information systems.

---

## 2. Development Environment

| Component | Technology |
|------------|------------|
| Ontology Language | OWL 2 |
| Serialization Format | RDF/XML |
| Ontology Editor | Protégé Desktop |
| Reasoner | HermiT |
| Ontology File | CulturalHeritageOntology_SMALL_30_CLASSES.owl |

---

## 3. How to Run the Ontology

### Step 1 – Install Protégé

Download Protégé Desktop from:

https://protege.stanford.edu/

### Step 2 – Open the Ontology

1. Launch **Protégé**.
2. Select **File → Open**.
3. Choose:

```text
CulturalHeritageOntology_SMALL_30_CLASSES.owl
```

### Step 3 – Explore the Ontology

After loading the ontology:

- Open the **Classes** tab.
- Open the **Object Properties** tab.
- Open the **Data Properties** tab.
- Open the **Individuals** tab.
- Review ontology metrics and hierarchy.

### Step 4 – Run the Reasoner

1. Click **Reasoner**.
2. Select **HermiT Reasoner**.
3. Click **Start Reasoner**.

### Step 5 – Verify Consistency

After reasoning:

- Inspect inferred class hierarchies.
- Review inferred relationships.
- Confirm that no inconsistencies are reported.

**Expected Result:**

The ontology should classify successfully and remain logically consistent.

---

## 4. Ontology Objectives

The ontology was developed to:

- Model cultural heritage knowledge semantically.
- Represent museum collections and exhibitions.
- Describe artworks and cultural artifacts.
- Support conservation and restoration activities.
- Enable semantic querying and reasoning.
- Facilitate interoperability between heritage information systems.

---

## 5. Conceptual Model

The ontology contains **30 Classes**.

### Heritage Resource Classes

- CulturalHeritageObject
- Artifact
- Artwork
- Painting
- Sculpture
- Manuscript
- Coin
- Textile
- HeritageSite

### Human and Organizational Classes

- Agent
- Artist
- Curator
- Conservator
- Researcher
- Museum
- CulturalInstitution

### Collection and Exhibition Classes

- Collection
- Exhibition
- Archive

### Contextual Classes

- HistoricalPeriod
- Event
- AcquisitionEvent
- RestorationEvent
- ExhibitionEvent
- Location
- Country
- City

### Documentation and Material Classes

- MediaObject
- Image
- Material

---

## 6. Semantic Relationships

The ontology defines object properties including:

- hasCreator
- displayedIn
- belongsToCollection
- associatedWithPeriod
- madeOf
- curatedBy
- organizedBy
- locatedIn
- documentedIn
- restoredBy
- restoresObject
- preservedBy
- references
- owns
- manages
- hasLocation
- participatesInEvent
- acquiresObject
- exhibitsObject
- hasPart

These relationships connect heritage resources with people, institutions, materials, events, collections, and locations.

---

## 7. Descriptive Attributes

Datatype properties include:

- hasTitle
- hasDescription
- inventoryNumber
- creationDate
- acquisitionDate
- conditionStatus
- height
- width
- estimatedValue
- fileFormat
- publicationYear
- materialType

---

## 8. Modeling Strategy

### Agent Abstraction

The superclass **Agent** is used to represent both people and organizations participating in museum activities.

### Cultural Object Modeling

The ontology separates artworks, artifacts, and heritage sites into specialized subclasses.

### Event-Based Representation

Acquisition, restoration, and exhibition activities are represented through dedicated event classes.

### Location Modeling

Countries and cities are represented as subclasses of **Location**.

### Digital Documentation

Media resources are modeled separately from physical cultural heritage objects.

---

## 9. OWL 2 Features Utilized

The ontology employs:

- Class hierarchies
- Subclass relations
- Object properties
- Datatype properties
- Domain restrictions
- Range restrictions
- Functional properties
- Inverse properties
- Transitive properties
- Symmetric properties
- Existential restrictions
- Disjoint classes
- Named individuals
- Ontology IRI declaration
- RDF/XML serialization

---

## 10. Sample Knowledge Graph

### The Starry Night

#### Individual

**TheStarryNight : Painting**

#### Relationships

- hasCreator → VincentVanGogh
- displayedIn → MuseumOfModernArt
- associatedWithPeriod → PostImpressionism
- madeOf → OilPaint

#### Attributes

- hasTitle = "The Starry Night"
- inventoryNumber = "MOMA-001"
- conditionStatus = "Stable"

---

### Mona Lisa

#### Individual

**MonaLisa : Painting**

#### Relationships

- hasCreator → LeonardoDaVinci
- displayedIn → LouvreMuseum
- associatedWithPeriod → Renaissance
- madeOf → OilPaint

#### Attributes

- hasTitle = "Mona Lisa"
- inventoryNumber = "LOUVRE-001"
- conditionStatus = "Protected"

---

## 11. Individuals Included

The ontology contains **13 Sample Individuals**:

- LeonardoDaVinci
- LouvreCollection
- LouvreMuseum
- MoMACollection
- MonaLisa
- MuseumOfModernArt
- NewYorkCity
- OilPaint
- ParisCity
- PostImpressionism
- Renaissance
- TheStarryNight
- VincentVanGogh

---

## 12. Consistency Verification

The ontology was validated using the **HermiT Reasoner** within **Protégé**.

### Validation Procedure

1. Load the ontology into Protégé.
2. Start the HermiT reasoner.
3. Execute ontology classification.
4. Review inferred hierarchies.
5. Check logical consistency.

### Result

**No logical inconsistencies were detected.**

The ontology is logically valid and compatible with **OWL 2 reasoning standards**.

---

## 13. Project Summary

The **Cultural Heritage and Museum Ontology** provides a structured semantic framework for representing cultural heritage assets, museum collections, artworks, artifacts, historical knowledge, conservation records, and digital documentation resources.

The ontology supports:

- Knowledge organization
- Semantic interoperability
- Museum collection management
- Heritage preservation workflows
- Digital heritage documentation
- Automated semantic reasoning

The final ontology is fully compliant with **OWL 2 standards** and demonstrates ontology engineering principles within the **Cultural Heritage Domain**.
