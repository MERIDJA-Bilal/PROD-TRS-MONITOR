# PROD-TRS-MONITOR
Suivi et pilotage du TRS à partir des rapports de production

Ce projet consiste en le développement d'un outil léger de suivi de la performance industrielle, permettant de collecter, exploiter et analyser les données de production issues des rapports de poste afin de piloter les lignes de fabrication.

L'outil permet de :

Importer les rapports de production par simple glisser-déposer, en lot
Extraire automatiquement les données clés de chaque rapport : production, qualité, arrêts machine, défauts et références fabriquées
Reprendre le TRS (Taux de Rendement Synthétique) tel que calculé par le système de production, sans recalcul, et reconstruire sa décomposition disponibilité, performance et qualité
Consolider l'historique des postes et suivre les indicateurs sur une période paramétrable, avec filtres par vacation, chantier et référence
Analyser la performance par référence, comparer les vacations, classer les postes et identifier les pannes et défauts récurrents par analyse de Pareto
Mettre en évidence la cadence de référence implicite de chaque produit, afin de détecter toute dérive du paramétrage du référentiel
Exporter les données consolidées aux formats CSV et JSON pour exploitation externe

L'objectif principal est de transformer des rapports de production isolés en indicateurs de performance fiables et exploitables, afin d'optimiser le pilotage des lignes industrielles et d'identifier rapidement les leviers de progrès.
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
OEE Monitoring & Performance Management from production reports

This project involves the development of a lightweight industrial performance monitoring tool designed to collect, process, and analyze production data extracted from shift reports in order to improve production line management.

The tool enables:

Importing production reports through drag and drop, in batch
Automatically extracting key data from each report: output, quality, machine downtime, defects and manufactured references
Taking OEE (Overall Equipment Effectiveness) as calculated by the production system, without recalculation, and reconstructing its availability, performance and quality breakdown
Consolidating shift history and tracking indicators over a configurable period, with filters by shift, work area and product reference
Analyzing performance by product reference, comparing shifts, ranking individual runs and identifying recurring failures and defects through Pareto analysis
Surfacing the implicit reference cycle time of each product, making any master data drift immediately detectable
Exporting consolidated data in CSV and JSON formats for external use

The main objective is to transform isolated production reports into reliable and actionable performance indicators, helping optimize production line management and quickly identify improvement opportunities.

Technique

Application web autonome, un seul fichier HTML. Traitement intégralement local au navigateur : aucune donnée de production n'est transmise. Lecture des PDF par pdf.js, restitution graphique par Chart.js.

Standalone single-file web application. Fully client side processing, no production data transmitted. PDF parsing with pdf.js, charting with Chart.js.
