Example BarcodeSet XML::

  <?xml version="1.0" encoding="utf-8"?>
  <BarcodeSet xmlns="http://pacificbiosciences.com/PacBioDataModel.xsd" MetaType="PacBio.DataSet.BarcodeSet" Name="DataSet_BarcodeSet" Tags="barcode moreTags mapping mytags" UniqueId="b095d0a3-94b8-4918-b3af-a3f81bbe519c" Version="2.3.0" CreatedAt="2015-01-27T09:00:01" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://pacificbiosciences.com/PacBioDataModel.xsd">
    <ExternalResources>
      <ExternalResource Name="First Barcodes FASTA" Description="Points to an example Barcodes FASTA file." MetaType="PacBio.BarcodeFile.BarcodeFastaFile" ResourceId="file:///mnt/path/to/barcode.fasta" Tags="Example"/>
    </ExternalResources>
    <DataSetMetadata>
      <TotalLength>400</TotalLength>
      <NumRecords>30</NumRecords>
      <BarcodeConstruction>paired</BarcodeConstruction>
    </DataSetMetadata>
  </BarcodeSet>
