# MaltBarley_ConsumerPanel_HotsteepBeer
Supporting data and R code for Craine et al., 2021 (https://doi.org/10.1111/1750-3841.15786)

R markdown files (.Rmd) feature the following statistical analyses:
    -analysis of variance (ANOVA) and visualization of effects
    -correlation between hot steep and beer liking
    -principal component analysis (PCA) of malt quality, hot steep and beer liking
    -analysis of check-all-that-apply (CATA) data using a contingency table, correspondence analysis, and visualization with symmetric and asymmetric biplots
    -correlation between hot steep and beer CATA, and between malt quality and liking/sensory attributes
    -text mining and visualization using open comments from beer tasting
    -consumer clustering based on demographics, consumption patterns, liking
    -analysis of rank data (Friedman's test with posthoc analysis using Nemenyi Test)
    -multiple correspondence analysis (MCA)
    -Cochran’s Q-test and critical difference (Sheskin) procedure


Files
  -2017CCRUMaltQuality.Rmd
    -Replicated malt quality data provided by the United States Department of Agriculture (USDA) Cereal Crops Research Unit (CCRU)
     -Questions:
      -How do Entry and Rep influence malt quality traits?
      -How are malt quality traits related?
    -requires: 2017CCRU_MaltQuality.csv
  
  -2017MaltQualityComp.Rmd
    -Replicated malt quality data provided by USDA CCRU (uniform malting conditions) and Hartwick College Center for Craft Food and Beverage (malting conditions modified       for each genotpye
     -Questions:
        -How does entry and maltster influence malt quality traits?
        -How are malt quality traits related?
      -requires: MaltsterCompComb.csv
  
  -2017SensoryConsumerPanel_Beer.Rmd
    -analysis of consumer panel day 2 (beer tasting)
    -requires: BeerMasterCluster.csv; Pay6_long.csv; PayTableWide.csv; BeerOverallLiking_Cluster_CI.csv; BeerCATAV3.csv; OSUmalts.csv; BrewStatsCombined.csv;      BeerCATAV2.csv; BeerClusterPrep.csv; PrefMapBeerY.csv; PrefMapBeerY_90.csv; B.Atts_clean.csv; BeerMasterText.csv; ScreenerMasterwCluster.csv
  
  -2017SensoryConsumerPanel_HotSteep.Rmd
    -analysis of consumer panel day 1 (hot steep tasting)
    -requires: HotSteepMaster.csv; MaltsterCompComb_HartwickOSU.csv; OSUmalts.csv; HotSteepCATAV2.csv; HS.Atts.clean.csv

  -2017SensoryConsumerPanel_Combined.Rmd
    -combines analysis of data from hot steep and beer panels
    -requires: CombinedMaster.csv; CombinedMasterWide.csv; MeanSum_HS_B_Atts_clean.csv; MeanSum_HS_B_Atts_wide_clean.csv
    
  -2017SensoryConsumerPanel_Screener.Rmd
    -analysis of data from screener, including demographics and consumption patterns
    -requires: ScreenerMaster.csv; ScreenerQ9wide.csv; Screener_Q12.csv; ScreenerMasterwCluster.csv; ScreenerMasterwCluster.csv
  
  -2017SensoryConsumerPanel_ScreenerLiking.Rmd
    -analysis of influence of screener variables on liking
    requires: CombinedMasterWide.csv; ConsumerPanel_CodedScreener_YesNoCoded.csv; CombinedMasterWide.csv; ScreenerMaster.csv; BeerMasterCluster.csv; 
    
  -XLSTAT_BeerCATA_V3.xlsm
    -analysis of beer check-all-that-apply (CATA) in Excel, using XLSTAT
  -XLSTAT_HotSteepCATA_V3.xlsx
    -analysis of hot steep check-all-that-apply (CATA) 
  -XLSTAT_MaltQuality_CATA_Liking.xlsm
    -analysis of malt quality and beer/hot steep liking/sensory attributes (CATA) in Excel, using XLSTAT
  -Beer_OverallLiking_ConsumerClusterAnalysis.xlsx
    -consumer cluster analysis based on beer overall liking in Excel, using XLSTAT 
