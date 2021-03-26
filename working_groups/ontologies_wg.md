---
layout: page
title: Technical WG - Ontologies
permalink: /ontologies_wg/
---

# Technical WG 1 - Ontologies

Provide short description of the working group, its aims.

=======
This document official draft is stored in Zenodo at <span>doi:</span><span class="c61">[10.5281/zenodo.4639507](https://www.google.com/url?q=https://doi.org/10.5281/zenodo.4639507&sa=D&source=editors&ust=1616770309979000&usg=AOvVaw2qjGzKUyMmqXPbE1Q3yOFo)</span>


# <span>Modeling Epigraphy with an Ontology</span>
<span>Contributors</span><span>&nbsp;(alphabetically ordered by </span><span>surname</span><span>):</span><sup>[[1]](#ftnt1)</sup><span>&nbsp;</span>

<span class="c12">[Gabriel Bodard](https://www.google.com/url?q=https://wiki.digitalclassicist.org/User:GabrielBodard&sa=D&source=editors&ust=1616770309980000&usg=AOvVaw023e9m-eVjZ9Bn-1QU7Xmj)</span><span>, Hugh Cayless, </span><span class="c12">[Chiara Cenati](https://www.google.com/url?q=https://orcid.org/0000-0003-4962-9611&sa=D&source=editors&ust=1616770309981000&usg=AOvVaw1XQeMtT7ON487gE8Lbze2f)</span><span>,</span><sup>[[2]](#ftnt2)</sup><span>&nbsp;Alison Cooley, Tom Elliott, Silvia Evangelisti, Achille Felicetti, </span><span class="c17 c27">Paula Granados, </span><span>Frank Grieshaber, Ethan Gruber, </span><span class="c12">[Aaron Hershkowitz](https://www.google.com/url?q=https://orcid.org/0000-0002-9456-8574&sa=D&source=editors&ust=1616770309981000&usg=AOvVaw2PYrPNTM0o_uRNFrS4obG2)</span><span>,</span><sup>[[3]](#ftnt3)</sup><span>&nbsp;</span><span class="c17 c27">Tim Hill, </span><span class="c12 c27">[Harri Kiiskinen](https://www.google.com/url?q=https://orcid.org/0000-0003-4187-5551&sa=D&source=editors&ust=1616770309981000&usg=AOvVaw2rZQ9gRqRzWVdwWdfzZ550)</span><sup class="c17 c27">[[4]](#ftnt4)</sup><span class="c17 c27">, </span><span>Thomas Kollatz, Adeline Levivier, </span><span class="c12">[Pietro Liuzzo](https://www.google.com/url?q=https://orcid.org/0000-0001-5714-4011&sa=D&source=editors&ust=1616770309982000&usg=AOvVaw0CjL7W1NPdeIiIlMSac_Z9)</span><span>,</span><sup>[[5]](#ftnt5)</sup><span>&nbsp;</span><span class="c17 c27">Franco Luciani, </span><span>Andrea Mannocci, </span><span class="c17 c27">Emilia Mataix,</span><span>&nbsp;Francesca Murano, </span><span class="c17 c27">Orla Murphy,</span><span>&nbsp;</span><span class="c12">[Elli Mylonas](https://www.google.com/url?q=https://orcid.org/0000-0002-0215-4324&sa=D&source=editors&ust=1616770309983000&usg=AOvVaw2QNHvIEhPvFXz9f9N7GJmx)</span><span>, Jonathan Prag, Vincent Razanajao, Simona Stoyanova, </span><span class="c12">[Georgios Tsolakis](https://www.google.com/url?q=https://orcid.org/0000-0001-9555-4038&sa=D&source=editors&ust=1616770309983000&usg=AOvVaw0lEnUCf99NWpZ5fwrjvpbe)</span><span>,</span><sup>[[6]](#ftnt6)</sup><span>&nbsp;</span><span class="c17 c27">Charlotte Tupman, Irene Vagionakis, </span><span>Valeria Vitale, </span><span class="c17 c27">Franziska Weise.</span>
## <span>Table of C</span><span class="c22 c38">ontents</span>
<span class="c29 c17 c27 c40"></span>

<span class="c29 c31 c19 c17">[Modeling Epigraphy with an Ontology](#h.pri3k7e0bdkb)</span><span class="c29 c31 c19 c17">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c29 c19 c17 c31">[1](#h.pri3k7e0bdkb)</span>

<span class="c4">[Table of Contents](#h.ue1ixpsgcrqv)</span><span class="c4">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c4">[1](#h.ue1ixpsgcrqv)</span>

<span class="c17">[This document describes how to use existing ontologies as well as a few new properties and classes, to model epigraphic objects. Inscriptions that are described using this model can be shared, ingested into an ontological database, and used in graph databases or to share linked open data. Describing an inscription in this way complements existing practices as described by EpiDoc.](#h.rypca9sldjgc)</span><span class="c17">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c17">[2](#h.rypca9sldjgc)</span>

<span class="c4">[Prefixes](#h.t0cbd6nifnow)</span><span class="c4">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c4">[3](#h.t0cbd6nifnow)</span>

<span class="c4">[Added features of the Epigraphic Ontology](#h.yaqh7mvko4s8)</span><span class="c4">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c4">[4](#h.yaqh7mvko4s8)</span>

<span class="c4">[Classes](#h.86qcwvbgjous)</span><span class="c4">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c4">[4](#h.86qcwvbgjous)</span>

<span class="c4">[Properties](#h.p08ytaom23zw)</span><span class="c4">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c4">[4](#h.p08ytaom23zw)</span>

<span class="c4">[Modeling information](#h.surggcabc12b)</span><span class="c4">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c4">[5](#h.surggcabc12b)</span>

<span class="c4">[The Monument / Object](#h.ur43clqz9m1g)</span><span class="c4">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c4">[7](#h.ur43clqz9m1g)</span>

<span class="c4">[Facsimiles/Surrogates](#h.1mkfhqbc4ss6)</span><span class="c4">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c4">[9](#h.1mkfhqbc4ss6)</span>

<span class="c4">[Images](#h.bcxaz7aatclm)</span><span class="c4">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c4">[11](#h.bcxaz7aatclm)</span>

<span class="c4">[Places](#h.ufmkg27e7yln)</span><span class="c4">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c4">[12](#h.ufmkg27e7yln)</span>

<span class="c4">[The Inscription Text](#h.pd99nf6rxn2h)</span><span class="c4">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c4">[13](#h.pd99nf6rxn2h)</span>

<span class="c4">[The writing field](#h.nvnnmht6tqkm)</span><span class="c4">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c4">[14](#h.nvnnmht6tqkm)</span>

<span class="c4">[Fragments](#h.dnbuy269scj5)</span><span class="c4">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c4">[14](#h.dnbuy269scj5)</span>

<span class="c4">[Writing](#h.h08jvdjw20q0)</span><span class="c4">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c4">[15](#h.h08jvdjw20q0)</span>

<span class="c4">[Phases of Execution](#h.3t422x3zf47l)</span><span class="c4">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c4">[16](#h.3t422x3zf47l)</span>

<span class="c4">[Reading](#h.s40p2u7gfuae)</span><span class="c4">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c4">[16](#h.s40p2u7gfuae)</span>

<span class="c4">[Transcription](#h.d7jwsz7rszci)</span><span class="c4">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c4">[17](#h.d7jwsz7rszci)</span>

<span class="c4">[Edition](#h.srxc1d6gan5k)</span><span class="c4">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c4">[18](#h.srxc1d6gan5k)</span>

<span class="c4">[Translation](#h.vdcjtpg919s)</span><span class="c4">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c4">[18](#h.vdcjtpg919s)</span>

<span class="c4">[Attestations](#h.ewkq9lvwbjbg)</span><span class="c4">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c4">[18](#h.ewkq9lvwbjbg)</span>

<span class="c4">[Sameness](#h.iuqqs353pspn)</span><span class="c4">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c4">[19](#h.iuqqs353pspn)</span>

<span class="c4">[Concepts in the EAGLE Vocabularies](#h.v43cwspr4co5)</span><span class="c4">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c4">[20](#h.v43cwspr4co5)</span>

<span class="c4">[Contributors](#h.8xk8xxxqmz9h)</span><span class="c4">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c4">[21](#h.8xk8xxxqmz9h)</span>

<span class="c4">[Reification (about that triple...)](#h.9dfbc7g82okw)</span><span class="c4">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c4">[21](#h.9dfbc7g82okw)</span>

<span class="c4">[The Many Missing Parts](#h.lc05u52onr3p)</span><span class="c4">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c4">[21](#h.lc05u52onr3p)</span>

<span class="c4">[Summary of Classes and Property](#h.3bw3nnslq6el)</span><span class="c4">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="c4">[23](#h.3bw3nnslq6el)</span>

<span class="c51 c62 c17 c27"></span>

<span class="c51 c17 c27 c62"></span>
- - -
## <span class="c41">This document describes how to use existing ontologies as well as a few new properties and classes, to model epigraphic objects. Inscriptions that are described using this model can be shared, ingested into an ontological database, and used in graph databases or to share linked open data. Describing an inscription in this way complements existing practices as described by EpiDoc.</span><sup class="c41">[[7]](#ftnt7)</sup>
### <span class="c25">Prefixes</span>
<span>Prefixes used in the following examples are all listed here for convenience. The empty namespace is the area of definition of local </span><span>entities</span><span class="c0">.</span>

<span class="c0"></span>

<span class="c0">@prefix : &lt;&gt; .</span>

<span>@prefix tm: &nbsp;&lt;</span><span class="c12">[https://www.trismegistos.org/text/](https://www.google.com/url?q=https://www.trismegistos.org/text/&sa=D&source=editors&ust=1616770309998000&usg=AOvVaw0iCLxXdk6lrqYVj4Dqy-aZ)</span><span class="c0">&gt; .</span>

<span>@prefix rdfs: &lt;</span><span class="c12">[http://www.w3.org/2000/01/rdf-schema#](https://www.google.com/url?q=http://www.w3.org/2000/01/rdf-schema%23&sa=D&source=editors&ust=1616770309998000&usg=AOvVaw31zsVGJH6NBq9uiDXmsUIa)</span><span class="c0">&gt; .</span>

<span>@prefix rdf: &lt;</span><span class="c12">[http://www.w3.org/1999/02/22-rdf-syntax-ns#](https://www.google.com/url?q=http://www.w3.org/1999/02/22-rdf-syntax-ns%23&sa=D&source=editors&ust=1616770309999000&usg=AOvVaw2TFcxTAeFBLIkWaCFPu2RL)</span><span class="c0">&gt; .</span>

<span>@prefix dc: &lt;</span><span class="c12">[http://purl.org/dc/elements/1.1/](https://www.google.com/url?q=http://purl.org/dc/elements/1.1/&sa=D&source=editors&ust=1616770310000000&usg=AOvVaw0lryj-87qiofDbKkBm8MQd)</span><span class="c0">&gt; .</span>

<span>@prefix dcterms: &lt;</span><span class="c12">[http://purl.org/dc/terms/](https://www.google.com/url?q=http://purl.org/dc/terms/&sa=D&source=editors&ust=1616770310000000&usg=AOvVaw23EYHK7ytZdUogdzjVck1g)</span><span class="c0">&gt; .</span>

<span>@prefix xsd: &lt;</span><span class="c12">[http://www.w3.org/2001/XMLSchema#](https://www.google.com/url?q=http://www.w3.org/2001/XMLSchema%23&sa=D&source=editors&ust=1616770310001000&usg=AOvVaw2m6sB6J2GH675KKEfiLT-2)</span><span class="c0">&gt; .</span>

<span>@prefix owl: &lt;</span><span class="c12">[http://www.w3.org/2002/07/owl#](https://www.google.com/url?q=http://www.w3.org/2002/07/owl%23&sa=D&source=editors&ust=1616770310002000&usg=AOvVaw2rL3g2SF0uR2dTwXTgINrG)</span><span class="c0">&gt; .</span>

<span>@prefix skos: &lt;</span><span class="c12">[http://www.w3.org/2004/02/skos/core#](https://www.google.com/url?q=http://www.w3.org/2004/02/skos/core%23&sa=D&source=editors&ust=1616770310002000&usg=AOvVaw0s2gOSSd1niIRc3jD9DTwu)</span><span class="c0">&gt; .</span>

<span>@prefix frbr: &lt;</span><span class="c12">[http://purl.org/vocab/frbr/core#](https://www.google.com/url?q=http://purl.org/vocab/frbr/core%23&sa=D&source=editors&ust=1616770310003000&usg=AOvVaw0QEIC3FqtQdI3HZsHnP73E)</span><span class="c0">&gt; .</span>

<span>@prefix nmo: &lt;</span><span class="c12">[http://nomisma.org/ontology#](https://www.google.com/url?q=http://nomisma.org/ontology%23&sa=D&source=editors&ust=1616770310003000&usg=AOvVaw1-hybtaA7w6crBJfEow1zU)</span><span class="c0">&gt; .</span>

<span>@prefix lawd: &lt;</span><span class="c12">[http://lawd.info/ontology/](https://www.google.com/url?q=http://lawd.info/ontology/&sa=D&source=editors&ust=1616770310004000&usg=AOvVaw0SLHhb0GPOrjliviDdI7SK)</span><span class="c0">&gt; .</span>

<span>@prefix foaf: &lt;</span><span class="c12">[http://xmlns.com/foaf/0.1/](https://www.google.com/url?q=http://xmlns.com/foaf/0.1/&sa=D&source=editors&ust=1616770310004000&usg=AOvVaw3M5wn4yNOSlrUUsF1C4YW-)</span><span class="c0">&gt; .</span>

<span>@prefix gn: &lt;</span><span class="c12">[http://www.geonames.org/ontology#](https://www.google.com/url?q=http://www.geonames.org/ontology%23&sa=D&source=editors&ust=1616770310005000&usg=AOvVaw2maCA20IicNXKpqVVDyqZT)</span><span class="c0">&gt; .</span>

<span>@prefix gndo: &lt;</span><span class="c12">[http://d-nb.info/standards/elementset/gnd#](https://www.google.com/url?q=http://d-nb.info/standards/elementset/gnd%23&sa=D&source=editors&ust=1616770310006000&usg=AOvVaw2JUhFxY9IOkUDad1lOIk7_)</span><span class="c0">&gt; .</span>

<span>@prefix geo: &lt;</span><span class="c12">[http://www.opengis.net/ont/geosparql#](https://www.google.com/url?q=http://www.opengis.net/ont/geosparql%23&sa=D&source=editors&ust=1616770310006000&usg=AOvVaw3CI31kBLEqzXhtzCoqp-xF)</span><span class="c0">&gt; .</span>

<span>@prefix edh: &lt;</span><span class="c12">[http://edh-www.adw.uni-heidelberg.de/edh/ontology#](https://www.google.com/url?q=http://edh-www.adw.uni-heidelberg.de/edh/ontology%23&sa=D&source=editors&ust=1616770310007000&usg=AOvVaw1M98sL-aYHkZEpcozMjuJh)</span><span class="c0">&gt; .</span>

<span>@prefix epnet: &lt;</span><span class="c12">[http://www.semanticweb.org/ontologies/2015/1/EPNet-ONTOP_Ontology](https://www.google.com/url?q=http://www.semanticweb.org/ontologies/2015/1/EPNet-ONTOP_Ontology&sa=D&source=editors&ust=1616770310008000&usg=AOvVaw3fz23cMeGfQNpbnYwqNaki)</span><span class="c0">#&gt; . </span>

<span>@prefix edm: &lt;</span><span class="c12">[http://www.europeana.eu/schemas/edm/](https://www.google.com/url?q=http://www.europeana.eu/schemas/edm/&sa=D&source=editors&ust=1616770310008000&usg=AOvVaw3moG5YlmBvXbWI_Ic5kRgw)</span><span class="c0">&gt; .</span>

<span>@prefix svcs: &lt;</span><span class="c12">[http://rdfs.org/sioc/services#](https://www.google.com/url?q=http://rdfs.org/sioc/services%23&sa=D&source=editors&ust=1616770310009000&usg=AOvVaw3jCt_nDflNSNIISj2FHOdj)</span><span class="c0">&gt; .</span>

<span>@prefix doap: &lt;</span><span class="c12">[http://usefulinc.com/ns/doap#](https://www.google.com/url?q=http://usefulinc.com/ns/doap%23&sa=D&source=editors&ust=1616770310009000&usg=AOvVaw1Gx4_wHytihK7Y16CuZPUM)</span><span>&gt; .</span>

<span>@prefix crm: &lt;</span><span class="c12">[http://erlangen-crm.org/current/](https://www.google.com/url?q=http://erlangen-crm.org/current/&sa=D&source=editors&ust=1616770310010000&usg=AOvVaw2ycd6rJs6bxduLfuA7M4Zr)</span><span>&gt; .</span>

<span>@prefix crmtex: &lt;</span><span class="c12">[http://www.cidoc-crm.org/crmtex/](https://www.google.com/url?q=http://www.cidoc-crm.org/crmtex/&sa=D&source=editors&ust=1616770310011000&usg=AOvVaw2ERj7Zhc0h3dDKfD_6jZ_q)</span><span class="c0">&gt; .</span>

<span>@prefix crmsci: &lt;</span><span class="c12">[http://www.cidoc-crm.org/crmsci/](https://www.google.com/url?q=http://www.cidoc-crm.org/crmsci/&sa=D&source=editors&ust=1616770310011000&usg=AOvVaw0N8knfRE_2uAcAJExLeZgS)</span><span class="c0">&gt; .</span>

<span>@prefix extech: &lt;</span><span class="c12">[https://w3id.org/executionTechnique/ontology#](https://www.google.com/url?q=https://w3id.org/executionTechnique/ontology%23&sa=D&source=editors&ust=1616770310012000&usg=AOvVaw0q4cpivekv0OOIDh0G5imm)</span><span class="c0">&gt; .</span>

<span>@prefix eagle: &lt;</span><span class="c12">[https://www.eaglenetwork.eu/voc/writing/lod/](https://www.google.com/url?q=https://www.eaglenetwork.eu/voc/writing/lod/&sa=D&source=editors&ust=1616770310012000&usg=AOvVaw3vrZax71tVMQAVP5oo5Uc0)</span><span class="c0">&gt; .</span>

<span>@prefix eagleExTech: &lt;</span><span class="c12">[https://www.eagle-network.eu/voc/writing/lod/](https://www.google.com/url?q=https://www.eagle-network.eu/voc/writing/lod/&sa=D&source=editors&ust=1616770310013000&usg=AOvVaw0sjBCOTY0RVptW0miqLjVH)</span><span class="c0">&gt; . </span>

<span>@prefix eagleObjTyp: &lt;</span><span class="c12">[https://www.eagle-network.eu/voc/objtyp/lod/](https://www.google.com/url?q=https://www.eagle-network.eu/voc/writing/lod/&sa=D&source=editors&ust=1616770310013000&usg=AOvVaw0sjBCOTY0RVptW0miqLjVH)</span><span class="c0">&gt; .</span>

<span>@prefix eagleInsTyp: &lt;</span><span class="c12">[https://www.eagle-network.eu/voc/typeins/lod/](https://www.google.com/url?q=https://www.eagle-network.eu/voc/typeins/lod/&sa=D&source=editors&ust=1616770310014000&usg=AOvVaw0jmDOUEAShDP3irUl1jx63)</span><span class="c0">&gt; .</span>

<span>@prefix eagleMat: &lt;</span><span class="c12">[https://www.eagle-network.eu/voc/material/lod/](https://www.google.com/url?q=https://www.eagle-network.eu/voc/typeins/lod/&sa=D&source=editors&ust=1616770310014000&usg=AOvVaw0jmDOUEAShDP3irUl1jx63)</span><span class="c0">&gt; .</span>

<span class="c0">@prefix epont: &lt;https://w3id.org/epont/ontology/&gt; .</span>

<span class="c0"></span>

<span class="c0"></span>
### <span class="c25">Added features of the Epigraphic Ontology</span>
<span>The namespace of the ontology is </span><span class="c12">[https://w3id.org/epont/ontology/](https://www.google.com/url?q=https://w3id.org/epont/ontology/&sa=D&source=editors&ust=1616770310015000&usg=AOvVaw20nHOyQ-QOldCHZK03k8Fj)</span><span>&nbsp;. The OWL file is available here </span><span class="c12">[https://github.com/PietroLiuzzo/epiont/blob/master/OWL/epont.owl](https://www.google.com/url?q=https://github.com/PietroLiuzzo/epiont/blob/master/OWL/epont.owl&sa=D&source=editors&ust=1616770310015000&usg=AOvVaw0aJUGiEMSHk7JTEb_4wmQn)</span><span>&nbsp;; </span><span>it</span><span>&nbsp;imports the following implementation of the CRMtex </span><span class="c12">[https://github.com/PietroLiuzzo/epiont/blob/master/OWL/crmtex.owl](https://www.google.com/url?q=https://github.com/PietroLiuzzo/epiont/blob/master/OWL/crmtex.owl&sa=D&source=editors&ust=1616770310016000&usg=AOvVaw2_PR6ubFVlJqFQfz-pcIuE)</span>

<span class="c0"></span>

<span>Zenodo Storage of these two OWL files: </span><span class="c12">[https://zenodo.org/record/4444132#.YAISa8VKjRY](https://www.google.com/url?q=https://zenodo.org/record/4444132%23.YAISa8VKjRY&sa=D&source=editors&ust=1616770310017000&usg=AOvVaw0-1utOWJRA9sMDGy25C706)</span><span class="c0">&nbsp;</span>

<span class="c0"></span>
#### <span class="c6">Classes</span>
<span class="c19">epont:Edition</span>

<span>This s</span><span>ubclass of </span><span class="c28">lawd:Edition</span><span class="c0">&nbsp;is defined because the edition of an inscription is often an item in a corpus of inscriptions with a numeric identifier, or is published within a specific article which may or may not solely be devoted to that edition. This is a different concept from that of a critical edition or an edition of a book (for example).</span>
#### <span class="c6">Properties</span>
<span class="c19">epont:carriesText</span><span class="c0">&nbsp;</span>

<span>The Property </span><span class="c28">epOnt:carriesText</span><span>, is defined as the key Property to link objects and written texts, and is a subclass of </span><span class="c28">crm:P56_bears_feature (is found on</span><span>) instead of the </span><span class="c28">crm:P128_carries</span><span class="c0">&nbsp;as proposed in EPNet and EAGLE.</span>

<span class="c0"></span>

<span class="c29 c31 c19 c49">epont:hasEdition</span>

<span>This Property is a subclass of </span><span class="c28">crm:P94_has_created</span><span>&nbsp;and is used to connect an Activity of </span><span class="c28">TX6 Transcription</span><span>&nbsp;to the Edition of that transcription published somewhere. </span>

<span class="c0"></span>
- - -
## <span class="c22 c38"></span>
## <span class="c22 c38">Modeling information</span>
<span>The following is a summary depiction of the main entities involved in the model using generically understandable terms. In a nutshell, it takes the Inscription as studied by epigraphers as a pair of closely related but distinct entities, an Object and a Written Text. It is neither necessary nor desirable to prioritize either Text or Object, but the two must be distinguished in order to be accurately described. The Written Text and its fragments have been written in a series of execution phases to reproduce a Text. The scholar who observes the written text and the object may produce a transcription which may become part of an Edition and which may then be translated. </span><span>In this visual model no specific, formal, concept name is used; instead simplified labels are used to make the model clearer. The formal class and Property names appear in the examples and in the description.</span>

<span class="c0"></span>

<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 620.5px; height: 180.94px;"><img src='{{site.baseurl}}/assets/images/image4.png' style="width:100%;" alt="Text
 Images
 Execution
 Writing
 Period
 Translation
 Object Type
 Object
 Written Text
 Type of Text
 Edition
 Material
 Reading
 Transcription
 Places
 Field
" title="Overview of the ontology" align="middle"/></span>

<span class="c0"></span>

<span class="c0"></span>

<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 624px; height: 146.28px;"><img src='{{site.baseurl}}/assets/images/image18.png' style="width:100%;" alt="" title="" align="middle"/></span>

<span class="c0"></span>

<span>On finding a new inscription, its existence could be defined by the simple three instances and two relations seen above. However, because we are pretty sure it was written, the minimal set should actually have one more Property and one more entity.</span>

<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 537.05px; height: 261.64px;"><img src='{{site.baseurl}}/assets/images/image5.png' style="width:100%;" alt="Writing
 Object
 Written Text
 Reading
" title="Main concepts" align="middle"/></span>

<span class="c0"></span>

<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 624px; height: 233.31px;"><img src='{{site.baseurl}}/assets/images/image28.png' style="width:100%;" alt="" title="" align="middle"/></span>

<span class="c0"></span>

<span class="c0"></span>

<span class="c0"></span>
### <span class="c25">The Monument / Object</span>
<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 503.22px; height: 258.5px;"><img src='{{site.baseurl}}/assets/images/image6.png' style="width:100%;" alt="Images
 Period
 Object Type
 Object
 Written Text
 Material
 Places
" title="monument overview" align="middle"/></span>

<span class="c0"></span>

<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 623px; height: 235.6px;"><img src='{{site.baseurl}}/assets/images/image27.png' style="width:100%;" alt="" title="" align="middle"/></span>

<span class="c0"></span>

<span>The Object is a </span><span class="c16 c8">E22 Human-Made Object</span><span class="c16">&nbsp;</span><span>which is a subclass of </span><span class="c8">E19 Physical Object</span><span>&nbsp;</span><span>which is proposed in CRMtex. Not listed in the above model are all the more standard properties which can be attached to a </span><span class="c16 c8">E22 Human-Made Object</span><span>, like </span><span class="c8">crm:P48_has_preferred_identifier</span><span>&nbsp;or </span><span class="c8">crm:P104_is_subject_to</span><span>&nbsp;(for the rights) and which will also be omitted in the rest of the model examples. Similarly, the subproperties of </span><span class="c8">P4 has time span</span><span>&nbsp;can always be assigned to each of these objects. In this example, &nbsp;</span><span class="c8">dcterms:temporal</span><span>&nbsp;is used to link to a period entity, as in the Pelagios data </span><span>examples</span><span>. This serves as an additional piece of information, distinct from </span><span class="c8">P4 has time span</span><span class="c0">&nbsp;properties.</span>

<span class="c0"></span>

<span>The Object carries a Written Text (see </span><span class="c12">[The inscription](#h.pd99nf6rxn2h)</span><span>&nbsp;below</span><span>). The Property </span><span class="c8">epOnt:carriesText</span><span>&nbsp;is defined as the key Property to link objects and written texts, and is a subclass of </span><span class="c8">crm:P56_bears_feature (is found on)</span><span>. It is defined as a subProperty in order to distinguish it from </span><span class="c8">TXP2_is_included_within (included)</span><span>, which is also a subProperty of </span><span class="c8">crm:P56_bears_feature (is found on). </span><span>While </span><span class="c8">epOnt:carriesText</span><span>&nbsp;relates a </span><span class="c16 c8">E22 Human-Made Object</span><span class="c16">&nbsp;to a </span><span class="c16 c8">TX1 Written Text, </span><span class="c8">TXP2_is_included_within (included)</span><span class="c8 c16">&nbsp;</span><span class="c16">relates a </span><span class="c16 c8">TX1 Written Text </span><span class="c16">to a </span><span class="c16 c8">TX4 Writing Field</span><span>.</span>

<span class="c0"></span>

<span>The Property for the classification of monument or object type can also be attached to the object, and here the one proposed by EDH is reused and has been further specified as a subtype of </span><span class="c8">nmo:hasObjectType</span><span>. The range of the Property is a concept in the EAGLE Vocabulary. See below </span><span class="c12">[The Concepts in the EAGLE Vocabularies](#h.iuqqs353pspn)</span><span class="c0">. </span>

<span class="c0"></span>

<span>nmo:hasMaterial, which is declared in the ontology as a subProperty of </span><span class="c8">P45 consist of</span><span>&nbsp;is used in the same way as </span><span class="c8">edh:representsTypeOfMonument </span><span>to link to a concept defining a material (</span><span class="c8">E57 Material</span><span class="c0">). </span>

<span class="c0"></span>

<span>Dimensions of the object can be given using </span><span class="c8">P43 has dimension</span><span>&nbsp;and features of the decoration can also be added in pure CIDOC, as </span><span>&nbsp;in the EAGLE or EPNet models</span><span class="c0">.</span>

<span class="c0"></span>

<span>Several places can be specified by using the relevant properties defined by LAWD and linking to place entities defined locally or directly aligned to an available gazetteer, e.g. Pleiades or Trismegistos or any other relevant and open gazetteer (See below </span><span class="c12">[Places](#h.ufmkg27e7yln)</span><span>). While in this model </span><span class="c8">lawd:foundAt</span><span>&nbsp;and </span><span class="c8">lawd:origin</span><span>&nbsp;are used, the super-Property </span><span class="c8">lawd:where</span><span>&nbsp;</span><span class="c16">could also be used if neither of the previous two can be specified.</span><span>&nbsp;Only </span><span class="c8">lawd:foundAt </span><span>and not the super-Property </span><span class="c8">lawd:where</span><span>&nbsp;is equated to similar properties in other ontologies (</span><span class="c8">nmo:hasFindspot</span><span>&nbsp;and </span><span class="c8">epnet:hasFindingPlace</span><span>). </span><span class="c8">crm:P53 has former or current </span><span class="c8">location </span><span>is</span><span>&nbsp;</span><span>also </span><span>added t</span><span>o the range of subproperties of </span><span class="c8">lawd:where</span><span>, and includes the more specific subProperty used in the model, </span><span class="c8">P55 has current location</span><span class="c0">. </span>

<span class="c0"></span>

<span>The Property proposed by the epnet ontology to relate </span><span>bibliographic information to an entity</span><span>&nbsp;in a generic way (</span><span class="c8">epnet:isDocumentedBy</span><span>) is also used here as an example,</span><sup>[[8]](#ftnt8)</sup><span>&nbsp;to link the graph of this object to any list of identifiable bibliographic resources, distinct from any list of the editions of the text (see below </span><span class="c12">[The Edition](#h.srxc1d6gan5k)</span><span>), although potentially overlapping. The modeling of these bibliographic resources, if not directly pointing to standard RDF representations, should follow the FABIO</span><sup>[[9]](#ftnt9)</sup><span class="c0">&nbsp;or FRBR models. </span>

<span class="c0"></span>

<span>The Object inherits from the CRM implementation the core feature of modeling parts with </span><span class="c8">P46 is composed of</span><span class="c0">. To the example model above two further objects could be added as parts of the original object and modelled in the same way as that object, with or without a link to a Written Text. </span>

<span>Let us trace such an example now. Below we have two theorized fragments, se</span><span>parately described, transcribed and published</span><span class="c0">&nbsp;in different places . Each is modelled independently. </span>

<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 623px; height: 243.48px;"><img src='{{site.baseurl}}/assets/images/image30.png' style="width:100%;" alt="" title="" align="middle"/></span>

<span>Upon discovery that the two or more fragments belong to the same inscription, they could be joined by simply adding this statement to a further object entity (denoting the united object) or to one of the two. </span><span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 623px; height: 47.32px;"><img src='{{site.baseurl}}/assets/images/image16.png' style="width:100%;" alt="" title="" align="middle"/></span>

<span class="c0"></span>

<span>The Object is the only entity which can be possibly represented by an image or drawing (an abstraction of a text cannot be), and remains true also for objects which are drawings and sketches from field notes, for example. The images are linked with a standard CRM Property and defined as in the following section (</span><span class="c12">[Images](#h.1mkfhqbc4ss6)</span><span>).</span>
### <span>Facsimiles</span><span>/Surrogates</span>
<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 503.22px; height: 229.07px;"><img src='{{site.baseurl}}/assets/images/image13.png' style="width:100%;" alt="Object 
 Object 
 Reproduction
 Type
 Object
 Written Text
" title="reproductions" align="middle"/></span>

<span class="c0">Squeezes, Casts, 3D replicas and other types of reproductions are Objects as much as the original object or Text of which they are a copy.. It is sometimes the case that the only extant witness of a text is such a copy. A printed or digital image, if it is the only witness to an Object, is as such also an Object, and can be related to the abstract entity identifying the lost original. It is thus possible to clearly model whether a reading is based on the original object or on a copy. It is also possible to document the existence of such reproductions independently of whether they have been used for transcription or editing.</span>

<span class="c0"></span>

<span>At the same time, there must be a model for the relationships between the Objects. CIDOC </span><span class="c8">E-55_type</span><span class="c0">&nbsp;can be used to provide a list of types for this purpose.</span>

<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 623px; height: 389.38px;"><img src='{{site.baseurl}}/assets/images/image1.png' style="width:100%;" alt="" title="" align="middle"/></span>

<span class="c16">In the above example two Reproduction activities of the creation of a Squeeze and a Cast are defined and linked to an Object via </span><span class="c16 c8">P12 occurred in the presence of</span><span class="c16">.</span><sup class="c16">[[10]](#ftnt10)</sup><span class="c16">&nbsp;The creation of a reproduction is a Production (</span><span class="c16 c8">E12 Production</span><span class="c16">) which can be dated and can have an Actor, like any other activity, while the Object it produces is an Object like any other and can have the same properties as the Object on which it is based. Many of the properties listed under </span><span class="c16 c8">E12 Production</span><span class="c16 c29">&nbsp;in the CIDOC CRM documentation could also be used here, to document the facsimile production. The Cast and Squeeze defined in the example above are also objects which carry a written text. In the case of a lost inscription, for which only a Squeeze survives we could have the following modeling, although nothing would prevent the epOnt:carriesText Property from remaining attached to the 'original' object. A squeeze or photo of a plaster cast is also definable this way, and each object can have its own properties regarding material, dating, etc. The special status of the object used for reproductions is thus not defining.</span>

<span class="c16 c29"></span>

<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 623px; height: 386.42px;"><img src='{{site.baseurl}}/assets/images/image15.png' style="width:100%;" alt="" title="" align="middle"/></span>

<span>Additionally, as for images, </span><span class="c8">P138 represents (has representation)</span><span>&nbsp;can be used to link digital representations of any of these </span><span class="c8">E22_Human-Made_Object</span><span class="c0">, so that one can have, for example, a 3D model of a squeeze as well as a 3D model of the object on which that squeeze was made. </span>

<span class="c0"></span>

<span>Similarly, </span><span class="c8">E55 type</span><span class="c0">&nbsp;can be used to mark the best among many available objects related in this way. This allows us to precisely say if, for example, a reading has been made on a source which is not the best available. (Note that this kind of classification will necessarily be subjective.)</span>

<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 623px; height: 179.41px;"><img src='{{site.baseurl}}/assets/images/image26.png' style="width:100%;" alt="" title="" align="middle"/></span>

<span class="c0">These types are not defined in this ontology and depend on Vocabularies locally defined by data providers; they are important here only for their relation to one another.</span>
### <span class="c25">Images</span>
<span class="c0"></span>

<span>This model is entirely taken from Nomisma documentation, which was also expanded to include the way the EDM</span><sup>[[11]](#ftnt11)</sup><span class="c0">&nbsp;model represents links to IIIF images.</span>

<span class="c0"></span>

<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 624px; height: 205.33px;"><img src='{{site.baseurl}}/assets/images/image11.png' style="width:100%;" alt="" title="" align="middle"/></span>
### <span class="c25">Places</span>
<span>The modeling of the place concepts associated with an object or that appear in attestations is not within the scope of an epigraphic ontology. The example below is a light modification of the current model used by EDH, where the most important things are the class </span><span class="c8">lawd:Place</span><span>&nbsp;(equivalent to </span><span class="c8">E27_Site</span><span>) and the </span><span class="c8">owl:</span><span class="c8">sameAs</span><span class="c0">. As in Pelagios, SKOS properties can be used for matching and hierarchy.</span>

<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 624px; height: 208.95px;"><img src='{{site.baseurl}}/assets/images/image25.png' style="width:100%;" alt="" title="" align="middle"/></span>

<span>The Property </span><span class="c8">dcterms:isPartOf</span><span>&nbsp;is used instead of </span><span class="c8">skos:broader</span><span>&nbsp;as in the EDH </span><span>data</span><span class="c0">. The same place model can be used to model any place concept used in the information exposed.</span>

<span>A much richer description in RDF can be seen for example from Pleiades, e.g. </span><span class="c12">[https://pleiades.stoa.org/places/39271/turtle](https://www.google.com/url?q=https://pleiades.stoa.org/places/39271/turtle&sa=D&source=editors&ust=1616770310038000&usg=AOvVaw0mNFkNDT7PgR85t9GM1uOh)</span><span>.</span><sup>[[12]](#ftnt12)</sup>
### <span class="c25">The Inscription Text</span>
<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 537.05px; height: 265.5px;"><img src='{{site.baseurl}}/assets/images/image8.png' style="width:100%;" alt="Execution
 Writing
 Object
 Written Text
 Reading
 Field
" title="text of the inscription" align="middle"/></span>

<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 624px; height: 191px;"><img src='{{site.baseurl}}/assets/images/image9.png' style="width:100%;" alt="" title="" align="middle"/></span>

<span>In CRMtex, the class </span><span class="c8">TX1 Written Text</span><span>&nbsp;is the central point of definition of the inscription and is here equivalent to a </span><span class="c8">lawd:ConceptualWork</span><span>&nbsp;because it shares the same logic of detachment of the conceptual level from the text as reading, transcription or edition. The class </span><span class="c8">epnet:Inscription</span><span>&nbsp;is also aligned to this concept. Note that the </span><span class="c8">edh:Inscription</span><span>&nbsp;class is aligned to </span><span class="c8">TX6 Transcription</span><span class="c0">&nbsp;instead.</span>

<span class="c0">&nbsp;</span>

<span>For completeness, </span><span class="c8">P56 is found on</span><span>&nbsp;is repeated here </span><span>although redundant</span><span class="c0">. This is also to show that a provider of inscriptions as archived text could provide this information without offering any information about the object itself, leaving that part to others.</span>

<span class="c0"></span>

<span>Although the date of the text depends on its interpretation and thus on the Reading (see </span><span class="c12">[The reading](#h.s40p2u7gfuae)</span><span>), here an example is offered of how the nomisma properties </span><span class="c8">nmo:hasStartDate</span><span>&nbsp;and </span><span class="c8">nmo:hasEndDate</span><span>&nbsp;could be used to specify a date for the abstraction of the written text different from that of any writing / production or execution phase. These properties are both declared as subclasses of </span><span class="c8">P4 has time-span</span><span>&nbsp;</span><span class="c0">&nbsp;in this ontology.</span>

<span class="c0"></span>

<span>The </span><span class="c8">TX1 Written Te</span><span class="c8">xt</span><span>&nbsp;is the domain</span><span>&nbsp;of the Property </span><span class="c8">crmtex:TXP2 is included within</span><span>, which allows for the separate &nbsp;description of the </span><span class="c8">TX4 Writing Field</span><span>&nbsp;(</span><span class="c12">[The writing field](#h.nvnnmht6tqkm)</span><span>), as in the documentation of CRMtex. </span><span>In CRMtex a </span><span class="c8">TX1 Written Text</span><span>&nbsp;is linked to a class</span><span class="c8">&nbsp;TX2 Writing</span><span>&nbsp;by a </span><span class="c34 c27">specific Property </span><span class="c8 c34 c27">TXP5 was written by</span><span class="c34 c27">, subclass of </span><span class="c8 c27 c34">P108 was produced by</span><span class="c34 c27">,</span><span class="c34 c27">&nbsp;introduced to specify the particular relationship between the written text and the event that produced it.</span><span class="c8">TX1 Written Text</span><span>&nbsp;is also linked to</span><span>&nbsp;a </span><span class="c8">TX5 Reading</span><span>&nbsp;with a Property </span><span class="c26">introduced to specify the relationship between the written text and its reading: the </span><span class="c8 c26">TXP9 was read by</span><span class="c26">, subclass of</span><span>&nbsp;</span><span class="c8">O6 observed by</span><span>&nbsp;from the CRMsci module</span><span>&nbsp;(see </span><span class="c56">[The Reading](#h.s40p2u7gfuae)</span><span class="c0">). This is crucial to distinguish the text production from the investigation which leads to a transcription. It is necessary to abstract the text separately from its production aspect and transcription aspect to be able to associate the information precisely. This is an extremely important contribution from this model, which inherently allows the association of distinct and identifiable autopsies to a single text. It is thus possible to model the fact that a specific transcription is based on a specific autopsy event or instead is based on a previous edition, or on another Observation event. This is a major improvement possibility for the study of epigraphy, opening the path for attempts to disentangle the genesis of editions and publications.</span>

<span class="c0"></span>

<span>To the </span><span class="c8">TX4 Writing </span><span>events in this example a series of other Events are </span><span>also </span><span>linked using the </span><span class="c8">extech:hasExecutionPhase</span><span>&nbsp;Property, equivalent to </span><span class="c8">P31 has modified</span><span>.</span><span class="c8">&nbsp;</span><span>This allows the use of an event-based description structure for any </span><span class="c8">TX1 Written Text</span><span>.</span>
#### <span class="c6">The writing field</span>
<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 628px; height: 30.5px;"><img src='{{site.baseurl}}/assets/images/image17.png' style="width:100%;" alt="" title="" align="middle"/></span>

<span>The CRMtex class </span><span class="c8">TX4 Writing field</span><span>&nbsp;has already been discussed, &nbsp;and this model inherits that description as is. Like </span><span class="c8">TX1 Written Text</span><span>&nbsp;this is always a subclass of </span><span class="c8">E25 Man-made Feature</span><span>&nbsp;and shares all its features. An updated example based on the Arc of Constantine is in Felicetti and Murano 2020.</span><sup>[[13]](#ftnt13)</sup><span class="c0">&nbsp;</span>

<span class="c0"></span>
#### <span class="c6">Fragments</span>
<span>Another important feature of CRMtex is the class </span><span class="c8">TX7 Written Text Fragment</span><span class="c0">, which provides a way to be able to model fragments of text separately from parts of objects. </span>

<span class="c0"></span>

<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 624px; height: 58.62px;"><img src='{{site.baseurl}}/assets/images/image19.png' style="width:100%;" alt="" title="" align="middle"/></span>

<span class="c0"></span>

<span>The Property </span><span class="c8">TXP4 composes</span><span>&nbsp;provides the ability to have a separate model for each independent fragment and easily join the history of observation and publication of multiple fragments into one. Being able to identify a part of text would enable (for example) associating it with other parts of the same written text and easily modeling inscriptions in multiple languages or in multiple scripts (or both) by having a conceptualization for each part. Each Written Text or Written Text Fragment will have a &nbsp; </span><span class="c8">crm:P108_has_produced_(was_produced_by)</span><span>&nbsp;linked to a </span><span class="c8">TX2 Writing</span><span class="c0">&nbsp;event.</span>

<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 620.5px; height: 177.88px;"><img src='{{site.baseurl}}/assets/images/image10.png' style="width:100%;" alt="Object
 Object
 Written Text Fragment
 Execution
 Writing
 Object
 Written Text
 Object
 Written Text Fragment
 Reading
 Reading
 Field
" title="writing" align="middle"/></span>
### <span class="c25">Writing</span>
<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 624px; height: 151.99px;"><img src='{{site.baseurl}}/assets/images/image23.png' style="width:100%;" alt="" title="" align="middle"/></span>

<span class="c0"></span>

<span class="c8">TX2 Writing</span><span>&nbsp;is a subclass of </span><span class="c8">E12 Production</span><span>&nbsp;and can have identifiers and time related declarations associated with it. It can also make use of </span><span class="c8">crm:P120_occurs_before </span><span>to link to any other</span><span>&nbsp;</span><span class="c8">E2 Temporal entity</span><span class="c0">. This Property scope note says that </span>

<span class="c31 c8 c49 c51">a temporal gap exists between the end of A and the start of B. This Property is only necessary if the relevant time spans are unknown (otherwise the relationship can be calculated).</span>

<span>T</span><span class="c0">his is extremely important for chronologically placing one entity relative to another without making vague assertions about time-spans if such are not possible with a decent level of accuracy.</span>

<span class="c0"></span>

<span>The example for this model focuses on two features which are relevant to this entity’s class: the association of a Script and of a Linguistic Object. The latter is an abstract written work</span><span>&nbsp;(a </span><span class="c8">lawd:WrittenWork</span><span>&nbsp;or any of its subclasses) which embodies the TX1 or TX7 to which it is associated.</span>

<span class="c0"></span>

<span>The </span><span class="c8">E33 Linguistic Object</span><span>&nbsp;can then be used to join different entities such as any E33, using for example properties of the SAWS ontology as in the example.</span><sup>[[14]](#ftnt14)</sup><span class="c0">&nbsp;This linguistic object is also usefully different from any other linguistic object resulting from reading (observation) so that the distinction between the text of the inscription and the transcription of the text of the inscription (diplomatic, editorial, etc.) is guaranteed. This linguistic Object does not have a literal text associated with it in this model, because the only possible literal text is a result of an observation and a transcription, as exemplified in the CRMtex document.</span>
#### <span class="c6">Phases of Execution</span>
<span>While writing is a specific sort of Production activity for a Written Text, many execution phases may be additionally involved, which are here classified using a draft ontology proposal for execution technique, which defines a </span><span class="c8">extech:Phase</span><span>&nbsp;as equivalent to a </span><span class="c8">E11 Modification</span><span>&nbsp;(so that </span><span class="c8">TX2 Writing</span><span>&nbsp;is also an </span><span class="c8">extech:Phase</span><span class="c0">&nbsp;in the ontology)</span>

<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 624px; height: 78.67px;"><img src='{{site.baseurl}}/assets/images/image20.png' style="width:100%;" alt="" title="" align="middle"/></span>

<span>This relies on several specific types of execution techniques and tools used to accomplish them which have been defined and organized in the Eagle Vocabulary for execution technique (see </span><span class="c12">[Concepts in the EAGLE Vocabularies](#h.iuqqs353pspn)</span><span class="c0">) of inscriptions, in order to be able to specify better and avoid confusions between tool and technique or result and tool, for example.</span>
### <span class="c25">Reading</span>
<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 620.5px; height: 224.1px;"><img src='{{site.baseurl}}/assets/images/image3.png' style="width:100%;" alt="Text
 Execution
 Writing
 Translation
 Object
 Written Text
 Type of Text
 Edition
 Reading
 Transcription
 Field
" title="reading" align="middle"/></span>

<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 624px; height: 92.2px;"><img src='{{site.baseurl}}/assets/images/image31.png' style="width:100%;" alt="" title="" align="middle"/></span>

<span>The reading of an inscription is a scientific observation, and is defined in CRMTex as a subclass of</span><span class="c8">&nbsp;S4 Observation</span><span>. It can have all properties of other Temporal Entities. Here only the ones most salient to epigraphic research are used in the example. Note also that the person possibly related to the autopsy by </span><span class="c8">P14 carried out by (performed)</span><span>&nbsp;need not be the actual author of the transcription or of the edition, although this will be often the case. To this event further annotations, for example related to the phenomenology of reading, could also be added.</span><sup>[[15]](#ftnt15)</sup>

<span class="c0"></span>

<span class="c0">These entities are those which are more likely to be used in a DTS API presentation.</span>

<span>This is a different meaning of "reading" from what is intended as a reading e.g. in the TEI and EpiDoc guidelines for the element &lt;rdg&gt;.</span><sup>[[16]](#ftnt16)</sup><span>&nbsp;The scientific observation which is subclassed in </span><span class="c8">TX5 Reading </span><span>is one action of reading in its entirety,</span><sup>[[17]](#ftnt17)</sup><span class="c0">&nbsp;which may or may not result in a known transcription or an edition, which in turn will contain "readings" of specific pieces of the text.</span>
#### <span class="c6">Transcription </span>
<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 624px; height: 280.94px;"><img src='{{site.baseurl}}/assets/images/image2.png' style="width:100%;" alt="" title="" align="middle"/></span>

<span>The </span><span class="c8">TX6 Transcription</span><span>, product of a Reading (here called Autopsy could also in theory be another Activity such as reading an edition). This is the entity which most closely resembles the contents of a record in a digital epigraphy archive when viewed specifically from the landing page of an inscription. In this entity we have a series of standard dc statements including the link to a landing page, an identifier, and temporal properties. This entity is, however, still distinct from the Epigraphic Edition (</span><span class="c12">[edition](#h.srxc1d6gan5k)</span><span>) which it may produce and which is related to it with a special Property </span><span class="c8">epOnt:hasEdition</span><span>, defined as a subclass of </span><span class="c8">P94 created</span><span>. This allows for a text transcription to be available even before it is published, and to be easily distinguished from published transcriptions, whatever the format of publication. The transcription can take different forms and the EpNet ontology has defined a range of properties to associate to the results of this activity, including a Property to associate an EpiDoc transcription in XML. Only to this transcribed (and thus interpreted) text can a typology for a text (or more) be associated with the </span><span class="c8">edh:representsTypeOfInscription</span><span>,</span><span>&nbsp;one of the concepts defined in the EAGLE Vocabularies (see </span><span class="c12">[The Concepts in the EAGLE Vocabularies](#h.iuqqs353pspn)</span><span class="c0">). </span>

<span>Other properties such as </span><span class="c8">edh:hasWorkstatus</span><span>&nbsp;could be related to this entity, and in particular attestations (</span><span class="c12">[Attestations](#h.ewkq9lvwbjbg)</span><span class="c0">), which will be related to a specific Transcription or Edition if available. </span>

<span class="c0">&nbsp; </span>
#### <span class="c6">Edition</span>
<span class="c0">The Bibliographical Reference associated with an Epigraphic Edition need not be specified in full, as bibliographic information modeling is beyond the scope of this model, but an edited text of the inscription could be modelled here, instead of the transcription text, to distinguish the two.</span>

<span class="c0"></span>

<span>The edition of an inscription is often a part, with a numeric identifier, of a corpus of inscriptions, or is published within a specific article which may or may not solely be devoted to that edition. This is a different concept from that of a critical edition or of an edition of a book and has been specified as a subclass of </span><span class="c8">lawd:Edition</span><span class="c0">.</span>

<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 624px; height: 104.78px;"><img src='{{site.baseurl}}/assets/images/image22.png' style="width:100%;" alt="" title="" align="middle"/></span>

<span class="c0">One autopsy and consequent transcription can create several editions, which is an additional added potential of the model. Each Edition can be associated with a translation.</span>
#### <span class="c6">Translation</span>
<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 624px; height: 115.9px;"><img src='{{site.baseurl}}/assets/images/image7.png' style="width:100%;" alt="" title="" align="middle"/></span>
### <span class="c25">Attestations</span>
<span class="c0">Any attestation is modelled as required for NE attestations by Pelagios/SNAP/others attestation model in EPNet, etc. and can be referred exactly to an edition, a transcription or a translation.</span>

<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 380.5px; height: 232.78px;"><img src='{{site.baseurl}}/assets/images/image14.png' style="width:100%;" alt="Translation
 Edition
 Transcription
 Attestation
" title="attestations" align="middle"/></span>
### <span>Sameness</span>
<span class="c0">This section is work in progress, it will be included in future releases. It will include modeling of different kind of sameness (same edition, same inscription, etc.). </span>
### <span class="c25">Concepts in the EAGLE Vocabularies</span>
<span class="c0">The EAGLE Vocabularies are used and linked to, but are far from being an established resource even for epigraphic projects which have started digitally. IIP for example uses Getty ATT for Object typologies. The Getty ATT is however very wide, and the EAGLE Vocabularies may still be a better and simpler proxy for epigraphers. However, there is no limitation or boundary here, and other vocabularies can be used or aligned to the EAGLE vocabularies. </span>

<span class="c0"></span>

<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 624px; height: 114.67px;"><img src='{{site.baseurl}}/assets/images/image24.png' style="width:100%;" alt="" title="" align="middle"/></span>

<span class="c0"></span>

<span>This approach, with separate vocabularies </span><span class="c0">would have the advantage of being done once for everyone for non problematic cases, while one could still jump to another value or point to a different authority if unsatisfied. </span>

<span class="c0"></span>

<span class="c0">To complete the above examples, here are some concepts and execution phases using them. </span>

<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 624px; height: 330.67px;"><img src='{{site.baseurl}}/assets/images/image12.png' style="width:100%;" alt="" title="" align="middle"/></span>
### <span class="c25">Contributors</span>
<span>Persons involved in any stage and at any defined level can be modelled on the example of what EDH already does, using mainly </span><span class="c8">FOAF </span><span class="c0">properties. The following is a result of a DESCRIBE Query to the SPARQL endpoint, as an example.</span>

<span class="c0"></span>

<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 624px; height: 181.33px;"><img src='{{site.baseurl}}/assets/images/image21.png' style="width:100%;" alt="" title="" align="middle"/></span>

<span class="c0"></span>
### <span class="c25">Reification (about that triple...)</span>
<span>The issue of attribution of each RDF statement is solved with a process of adding triples which speak about triples, called reification. However, this risks to be never-ending, as one may start to wish for triples which speak about triples about other triples. Nomisma.org (example below) does not use reification for every single triple, but only where needed, and the same approach is used here with Contributors, Editors, etc.</span><sup>[[18]](#ftnt18)</sup><span>&nbsp;Nothing prevents anyone from implementing this however there is no need for </span><span>prescription </span><span class="c0">in this document.</span>

<span class="c0"></span>

<span style="overflow-x: hidden; overflow-y: hidden; display: inline-block; margin-top: 0px; margin-right: 0px; margin-bottom: 0px; margin-left: 0px; border-top-color: rgb(0, 0, 0); border-top-style: solid; border-top-width: 0px; border-right-color: rgb(0, 0, 0); border-right-style: solid; border-right-width: 0px; border-bottom-color: rgb(0, 0, 0); border-bottom-style: solid; border-bottom-width: 0px; border-left-color: rgb(0, 0, 0); border-left-style: solid; border-left-width: 0px; width: 624px; height: 120.32px;"><img src='{{site.baseurl}}/assets/images/image29.png' style="width:100%;" alt="" title="" align="middle"/></span>

<span class="c0"></span>
### <span class="c25">The Many Missing Parts</span>
<span class="c0">Many other aspects of information are not covered here and are either</span>

- <span class="c0">Already covered by one of the imported ontologies</span>
- <span class="c0">Still in need of modeling of any type or vocabularies/definitions</span>
- <span>Covered by other ontologies not used here. For example, </span><span class="c27">the Reading concept may be expanded upon using Classes and properties of the READ-IT Ontology.</span>

<span class="c0">The modularity of RDF allows this to happen as needed. </span>

<span class="c0"></span>
- - -
### <span class="c25"></span>
### <span>Summary of Classes and Property</span>
<span>Summary of Classes and Property and their “common denomination” which may eventually become a class name mapped to the reference entity. This is only a list of what is contained in this modeling document, the many ways in which this data can be expanded are not listed or </span><span>prescribed</span><span class="c0">, but are listed where known.</span>


|  **Class or Property**   |  **Current mapped name**   |**Epont proposed name (EN)**|


|Class|crm:E22 Human-Made|Object|

|Property|epont:carriesText|Carries text|

|Class|crmtex:TX1_Written_text|Written Text|

|Property|crmtex:TXP9_was_read_by|Was read by|

|Class|crmtex:TX5_Reading|Reading|

|Class|crmtex:TX2_Writing|Writing|

|Property|crmtex:TXP5_was_written_by|Was written by|

|Property|dcterms:temporal|Time range (period)|

|Property|edh:representsTypeOfMonument|Monument Type|

|Property|crm:P46_is_composed_of|Is composed of Object|

|Property|nmo:hasMaterial|Material|

|Property|lawd:foundAt|Findspot|

|Property|crm:P55_has_current_location|Current location|

|Property |epnet:isDocumentedBy|Bibliography|

|Property |crm:P138i_has_representation |Images|

|Property|crm:P56_is_found_on|Found on|

|Property|nmo:hasEndDate|Not after|

|Property|nmo:hasStartDate  |Not before|

|Property|crmtex:TXP2_is_included_within|Is included within|

|Property|crmtex:TXP5_was_written_by|Was written by|

|Property|extech:hasExecutionPhase|Has execution phase|

|Class|crmtex:TX4_Writing_field|Writing field|

|Class|crmtex:TX7_Written_Text_Fragment|Fragment|

|Property|crmtex:TXP4_composes|Composes|

|Class|crmtex:TX2_Writing|Writing|

|Property|crmtex:TXP1_used_writing_system  |Used writing system|

|Property|crm:P92_brought_into_existence|Brought into existence|

|Class|lawd:WrittenWork|Work|

|Class|extech:Phase|Phase of execution|

|Property|extech:resultsIn  |Results in|

|Property|extech:uses_technique|Uses technique|

|Property|crm:P20_had_specific_purpose|Had specific purpose|

|Property|crmtex:TXP3_is_rendered_by|Is rendered by|

|Property|crm:P14_carried_out_by|Carried out by|

|Class|crmtex:TX6_Transcription|Transcription|

|Property|dct:contributor      |Contributor|

Property|dct:date  |date|

|Property|dct:publisher  |publisher|

|Property|dct:isPartOf         |Is part of|

|Property|crm:P49_created         |created|

|Property|epOnt:hasEdition|Has edition|

|Property|edh:representsTypeOfInscription|Type of inscription|

|Property|lawd:hasAttestation|Has attestation|

|Class|crm:E33_Linguistic_Object|Linguistic object|

|Property|edh:hasDiplomaticText|Diplomatic edition|

|Property|epnet:hasTranscription|transcription|

|Property|epnet:hasSimplifiedTranscription|Simplified transcription|

|Class|epOnt:Edition|edition|

|Property|crm:P73_has_translation|Has translation|

|Property|edh:hasEditionText|Edition text|


- - -
<div>

[[1]](#ftnt_ref1)<span class="c11">&nbsp;The list includes participants to seminars and workshops related to this work. Please notify the mailing list Epigraphic Ontology WG &lt;</span><span class="c12 c11">[epont@googlegroups.com](mailto:epont@googlegroups.com)</span><span class="c22 c11">&gt; .</span>

</div><div>

[[2]](#ftnt_ref2)<span class="c11">&nbsp;Universität Wien, </span><span class="c12 c11">[ERC Advanced Grant Project MAPPOLA-Mapping Out the Poetic Landscapes of the Roman Empire](https://www.google.com/url?q=https://mappola.eu/&sa=D&source=editors&ust=1616770310125000&usg=AOvVaw1T7V0obWYArRrlWWcrTD_i)</span><span class="c22 c11">.</span>

</div><div>

[[3]](#ftnt_ref3)<span class="c11">&nbsp;The Institute for Advanced Study, </span><span class="c12 c11">[the Krateros Project](https://www.google.com/url?q=https://www.ias.edu/krateros&sa=D&source=editors&ust=1616770310125000&usg=AOvVaw3bsHtYY_Y9erMfgb4Da2MW)</span><span class="c11 c22">.</span>

</div><div>

[[4]](#ftnt_ref4)<span class="c22 c11">&nbsp;Dept. of Cultural History, University of Turku</span>

</div><div>

[[5]](#ftnt_ref5)<span class="c11">&nbsp;Universität Hamburg, </span><span class="c11 c27">&nbsp;</span><span class="c12 c11 c27">[Beta maṣāḥǝft: Manuscripts of Ethiopia and Eritrea (Schriftkultur des christlichen Äthiopiens und Eritreas: eine multimediale Forschungsumgebung)](https://www.google.com/url?q=https://www.betamasaheft.uni-hamburg.de/&sa=D&source=editors&ust=1616770310123000&usg=AOvVaw3rM2BRiDFDetJaa2aiTRa7)</span><span class="c11">. Contributor of the initial complete draft and structure.</span>

</div><div>

[[6]](#ftnt_ref6)<span class="c22 c11">&nbsp;Institute for the Study of the Ancient World, New York University</span>

</div><div>

[[7]](#ftnt_ref7)<span class="c11">&nbsp;</span><span class="c12 c11">[https://epidoc.stoa.org/gl/latest/](https://www.google.com/url?q=https://epidoc.stoa.org/gl/latest/&sa=D&source=editors&ust=1616770310126000&usg=AOvVaw0OqqhXDdvSIg15mQefrWZR)</span><span class="c22 c11">&nbsp;</span>

</div><div>

[[8]](#ftnt_ref8)<span class="c22 c11">&nbsp;CITO properties could also be used for this, to differentiate the different sources. This is the praxis for example in the Pleiades dataset.</span>

</div><div>

[[9]](#ftnt_ref9)<span class="c22 c11">&nbsp;(Peroni and Shotton 2012)</span>

</div><div>

[[10]](#ftnt_ref10)<span class="c22 c11">&nbsp;See CIDOC-CRM v.7 page xxix .</span>

</div><div>

[[11]](#ftnt_ref11)<span class="c11">&nbsp; </span><span class="c12 c11">[https://pro.europeana.eu/resources/standardization-tools/edm-documentation](https://www.google.com/url?q=https://pro.europeana.eu/resources/standardization-tools/edm-documentation&sa=D&source=editors&ust=1616770310119000&usg=AOvVaw2u7AV5xf18JG7BudzbJPBD)</span><span class="c11">&nbsp;</span>

</div><div>

[[12]](#ftnt_ref12)<span class="c11">&nbsp;Although Pleiades does not serve a SPARQL Endpoint, the data is all freely available and can be loaded locally to a triplestore for querying as </span><span class="c11">RDF</span><span class="c22 c11">.</span>

</div><div>

[[13]](#ftnt_ref13)<span class="c11">&nbsp;</span><span class="c12 c11">[http://www.semantic-web-journal.net/system/files/swj2509.pdf](https://www.google.com/url?q=http://www.semantic-web-journal.net/system/files/swj2509.pdf&sa=D&source=editors&ust=1616770310121000&usg=AOvVaw1KfaBEM1X_6UfIHPve3Dfl)</span><span class="c22 c11">&nbsp;</span>

</div><div>

[[14]](#ftnt_ref14)<span class="c11">&nbsp;The SAWS ontology </span><span class="c12 c11">[http://www.ancientwisdoms.ac.uk/method/ontology/](https://www.google.com/url?q=http://www.ancientwisdoms.ac.uk/method/ontology/&sa=D&source=editors&ust=1616770310120000&usg=AOvVaw3yR10HKCzzUhjgrCd1rX3H)</span><span class="c11">&nbsp;</span>

</div><div>

