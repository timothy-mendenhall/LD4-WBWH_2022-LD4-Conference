# LD4-WBWH_2022-LD4-Conference
Materials for the workshop hosted by the LD4 Wikibase Working Hour at the 2022 LD4 Conference on Linked Data

Useful links
============
- [Project page](<https://www.wikidata.org/wiki/Wikidata:WikiProject_LD4_Wikidata_Affinity_Group/Wikibase_and_WBStack_Working_Hours>) of the LD4 Wikibase Working Hour
- The [wikibase.cloud instance](https://ld4-wbs-test.wikibase.cloud/wiki/Main_Page) used in today's workshop
- [List of properties](https://ld4-wbs-test.wikibase.cloud/wiki/Special:ListProperties) used in our wikibase.cloud instance

Workshop section on querying
============================
- [Query service](https://ld4-wbs-test.wikibase.cloud/query/) of our wikibase.cloud instance
- [First query](/firstQuery_noPrefix_ld4-wbwh_2022-07-11.rq) with no prefixes
- [Second query](secondQuery_withPrefix_ld4-wbwh_2022-07-11.rq) with prefixes
- [Third query](thirdQuery_withVizualization_ld4-wbwh_2022-07-11.rq) with qualifier and visualization

Workshop section on QuickStatements
===================================
- [QuickStatements syntax reference page](https://www.wikidata.org/wiki/Help:QuickStatements)
- [Dataset](https://raw.githubusercontent.com/timothy-mendenhall/LD4-WBWH_2022-LD4-Conference/main/LD4-2022_WBWH_Dataset%20-%20ForQuickStatementsDemo.csv) used during the demo

Workshop section on OpenRefine
==============================
- [Docker Desktop](https://www.docker.com/products/docker-desktop/)
- [Section on reconciling with Wikibase](https://docs.openrefine.org/manual/wikibase/reconciling) in the OpenRefine User Manual
- [GitHub repo of the Wikibase reconciliation service](https://github.com/wetneb/openrefine-wikibase)
- [Jim Hahn's presentation](https://penno365-my.sharepoint.com/:p:/g/personal/jimhahn_upenn_edu/EYU6wRYeC4BJoXNQA76PPeoBHDNLiCATAbx-lxdm5rASaA?rtime=NhPcVGBJ2kg) on reconciling a Wikibase with data in OpenRefine
- [OpenRefine to Wikibase: data upload pipeline](https://en.wikiversity.org/wiki/OpenRefine_to_Wikibase:_Data_Upload_Pipeline#Reconcile_with_Wikibase)
- [TIB presentation](https://docs.google.com/presentation/d/13EXuFoe9uecSN7D6ufl4ogdutGwkpa2VtVwihPVN3ig/edit#slide=id.g104e7fdfe4a_0_0) on using OpenRefine with Wikibase instances
- [Sample Wikibase manifests](https://github.com/OpenRefine/wikibase-manifests) for use with OpenRefine
Code snippets and files used when setting up the reconciliation service
-----------------------------------------------------------------------
- `git clone https://github.com/wetneb/openrefine-wikibase`
- [Sample config file](config.py)
- `docker-compose up`
- [Browser page](http://localhost:8000/) of the reconciliation service
- http://localhost:8000/en/api : enter this URL when "adding a standard service" to OpenRefine
- cell.recon.match.id: extracts Q-number of the matched Wikibase item
- cell.recon.match.name: extracts the label of the matched Wikibase item
- [JSON manifest](ld4-wbCloud-test_manifest.json) used during demo
