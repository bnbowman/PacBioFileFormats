Example Transformed_rs_subreadSet XML::

  <?xml version="1.0" encoding="UTF-8"?>
  <HdfSubreadSet xmlns:uuid="java:java.util.UUID" xmlns:bax="http://whatever"
                 xmlns="http://pacificbiosciences.com/PacBioDataModel.xsd"
                 xmlns:xs="http://www.w3.org/2001/XMLSchema"
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
                 xmlns:fn="http://www.w3.org/2005/xpath-functions"
                 Name="Subreads from run&#xA;                r000004_42268_150307"
                 MetaType="PacBio.DataSet.SubreadSet"
                 Tags="pacbio.secondary.instrument=RS"
                 Version="0.5"
                 UniqueId="a8c1f8c5-a0ca-4a90-95c7-bc291c389e09">
     <ExternalResources>
        <ExternalResource MetaType="PacBio.SubreadFile.BaxFile"
                          ResourceId="file:///C:/Users/aklammer/aklammer_laptop_2015/aklammer_laptop_2015/depot/software/smrtanalysis/bioinformatics/doc/FileFormats/examples/datasets/Analysis_Results/rs.1.bax.h5"/>
        <ExternalResource MetaType="PacBio.SubreadFile.BaxFile"
                          ResourceId="file:///C:/Users/aklammer/aklammer_laptop_2015/aklammer_laptop_2015/depot/software/smrtanalysis/bioinformatics/doc/FileFormats/examples/datasets/Analysis_Results/rs.2.bax.h5"/>
        <ExternalResource MetaType="PacBio.SubreadFile.BaxFile"
                          ResourceId="file:///C:/Users/aklammer/aklammer_laptop_2015/aklammer_laptop_2015/depot/software/smrtanalysis/bioinformatics/doc/FileFormats/examples/datasets/Analysis_Results/rs.3.bax.h5"/>
     </ExternalResources>
     <DataSetMetadata>
        <TotalLength>50000000</TotalLength>
        <NumRecords>150000</NumRecords>
        <Collections>
           <CollectionMetadata Context="rs" InstrumentName="42268" InstrumentId="1">
              <InstCtrlVer>2.3.0.1.142990</InstCtrlVer>
              <SigProcVer>NRT@172.31.128.10:8082, SwVer=2301.142990, HwVer=1.0</SigProcVer>
              <RunDetails>
                 <RunId>r000004_42268_150307</RunId>
                 <Name>Inst42268-030715-2kb-P4-0.05nM-6Chips-FAT2_3</Name>
              </RunDetails>
              <WellSample Name="Inst42268-030715-2kb-P4-0.05nM-2Chips-FAT3">
                 <PlateId>Inst42268-030715-2kb-P4-0.05nM-6Chips-FAT2_3</PlateId>
                 <WellName>Inst42268-030715-2kb-P4-0.05nM-2Chips-FAT3</WellName>
                 <Concentration>0</Concentration>
                 <SampleReuseEnabled>false</SampleReuseEnabled>
                 <StageHotstartEnabled>true</StageHotstartEnabled>
                 <SizeSelectionEnabled>
                                  false
                              </SizeSelectionEnabled>
                 <UseCount>1</UseCount>
                 <Comments>Inst42268-030715-2kb-P4-0.05nM-2Chips-FAT3</Comments>
                 <BioSamplePointers>
                    <BioSamplePointer>ad236d1c-2dd2-444e-9001-bba691cedad8</BioSamplePointer>
                 </BioSamplePointers>
              </WellSample>
              <Automation>
                 <AutomationParameters>
                    <AutomationParameter/>
                 </AutomationParameters>
              </Automation>
              <CollectionNumber>6</CollectionNumber>
              <CellIndex>1</CellIndex>
              <CellPac Barcode="10078306255000000182317020825155"/>
              <Primary>
                 <AutomationName>BasecallerV1</AutomationName>
                 <ConfigFileName>2-0-0_P4-C2.xml</ConfigFileName>
                 <SequencingCondition/>
                 <ResultsFolder>Analysis_Results</ResultsFolder>
                 <CollectionPathUri>rsy://mp-rsync/vol55//RS_DATA_STAGING/42268/Inst42268-030715-2kb-P4-0.05nM-6Chips-FAT2_3_4/B01_2/</CollectionPathUri>
                 <CopyFiles>
                    <CollectionFileCopy>Fasta</CollectionFileCopy>
                 </CopyFiles>
              </Primary>
           </CollectionMetadata>
        </Collections>
        <BioSamples>
           <BioSample Name="Inst42268-030715-2kb-P4-0.05nM-2Chips-FAT3"
                      Description="Inst42268-030715-2kb-P4-0.05nM-2Chips-FAT3"
                      UniqueId="ad236d1c-2dd2-444e-9001-bba691cedad8"/>
        </BioSamples>
     </DataSetMetadata>
  </HdfSubreadSet>