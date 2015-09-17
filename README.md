# OWL2SPARQL
OWL To SPARQL Query Rewriter

This project is supposed to provide a simple converter from OWL axioms and OWL class expressions to SPARQL queries.

## From OWL axiom to SPARQL query

### Usage
```Java
// create the converter
OWLAxiomToSPARQLConverter converter = new OWLAxiomToSPARQLConverter("?s","?o");

// provide some OWL axiom using OWL API datastructures
OWLAxiom axiom = ...;

// convert the axiom into a SPARQLquery
String queryString = converter.convert(axiom);
```

## From OWL class expression to SPARQL query

### Usage
```Java
// create the converter
OWLClassExpressionToSPARQLConverter converter = new OWLClassExpressionToSPARQLConverter();

// provide some OWL class expression using OWL API datastructures
OWLClassExpression ce = ...;

// convert the class expression into a SPARQL query
String queryString = converter.convert(ce);
```