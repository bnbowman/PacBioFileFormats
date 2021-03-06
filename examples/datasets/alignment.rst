Example AlignmentSet XML::

  <?xml version="1.0" encoding="utf-8"?>
  <AlignmentSet xmlns="http://pacificbiosciences.com/PacBioDataModel.xsd" MetaType="PacBio.DataSet.AlignmentSet" Name="DataSet_AlignmentSet" Tags="barcode moreTags mapping mytags" UniqueId="b095d0a3-94b8-4918-b3af-a3f81bbe519c" Version="2.3.0" CreatedAt="2015-01-27T09:00:01" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://pacificbiosciences.com/PacBioDataModel.xsd">
      <ExternalResources>
          <ExternalResource Name="First Alignments BAM" Description="Points to an example Alignments BAM file." MetaType="PacBio.AlignmentFile.AlignmentBamFile" ResourceId="file:///mnt/path/to/alignments0.bam" Tags="Example">
              <FileIndices>
                  <FileIndex MetaType="PacBio.Index.PacBioIndex" ResourceId="file:///mnt/path/to/alignments0.pbi"/>
              </FileIndices>
          </ExternalResource>
          <ExternalResource Name="Second Alignments BAM" Description="Points to another example Alignments BAM file, by relative path." MetaType="PacBio.AlignmentFile.AlignmentBamFile" ResourceId="file:./alignments1.bam" Tags="Example">
              <FileIndices>
                  <FileIndex MetaType="PacBio.Index.PacBioIndex" ResourceId="file:///mnt/path/to/alignments1.pbi"/>
              </FileIndices>
          </ExternalResource>
      </ExternalResources>
      <DataSets>
          <DataSet UniqueId="ab95d0a3-94b8-4918-b3af-a3f81bbe519c" Version="2.3.0" Name="HighQuality Read Alignments">
              <ExternalResources>
                  <ExternalResource/> <!-- This is a hack to make alignment set validate. Clearly the labelled subset needs a little more thought. -->
              </ExternalResources>
              <Filters> <!-- These Filters are in addition to those above. This provides a means to subset and label the parent DataSet further. -->
                  <Filter>
                      <Properties>
                          <Property Name="rq" Value="0.85" Operator=">"/>
                      </Properties>
                  </Filter>
              </Filters>
          </DataSet>
          <DataSet UniqueId="ac95d0a3-94b8-4918-b3af-a3f81bbe519c" Version="2.3.0" Name="Alignments to chromosome 1">
              <ExternalResources>
                  <ExternalResource/>
              </ExternalResources>
              <Filters>
                  <Filter>
                      <Properties>
                          <Property Name="RNAME" Value="chr1" Operator="=="/>
                      </Properties>
                  </Filter>
              </Filters>
          </DataSet>
      </DataSets>
      <DataSetMetadata>
          <TotalLength>50000</TotalLength>
          <NumRecords>5000</NumRecords>
          <Provenance CreatedBy="AnalysisJob">
              <ParentTool Name="pbalign" Version="0.1.0" Description="pbalign subreads.dataset.xml reference.dataset.xml"/>
          </Provenance>
      </DataSetMetadata>
  </AlignmentSet>
