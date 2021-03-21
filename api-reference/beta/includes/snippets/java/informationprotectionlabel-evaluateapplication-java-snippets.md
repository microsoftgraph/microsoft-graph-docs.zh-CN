---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 844e237ad69b54994cdd226d2f33f9edc9af78ac
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960957"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("User-Agent", "ContosoLOBApp/1.0"));

ContentInfo contentInfo = new ContentInfo();
contentInfo.additionalDataManager().put("format@odata.type", new JsonPrimitive("#microsoft.graph.contentFormat"));
contentInfo.format = ContentFormat.DEFAULT;
contentInfo.identifier = null;
contentInfo.additionalDataManager().put("state@odata.type", new JsonPrimitive("#microsoft.graph.contentState"));
contentInfo.state = ContentState.REST;
contentInfo.additionalDataManager().put("metadata@odata.type", new JsonPrimitive("#Collection(microsoft.graph.keyValuePair)"));
LinkedList<KeyValuePair> metadataList = new LinkedList<KeyValuePair>();
KeyValuePair metadata = new KeyValuePair();
metadata.name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled";
metadata.value = "True";
metadataList.add(metadata);
KeyValuePair metadata1 = new KeyValuePair();
metadata1.name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method";
metadata1.value = "Standard";
metadataList.add(metadata1);
KeyValuePair metadata2 = new KeyValuePair();
metadata2.name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate";
metadata2.value = "1/1/0001 12:00:00 AM";
metadataList.add(metadata2);
KeyValuePair metadata3 = new KeyValuePair();
metadata3.name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId";
metadata3.value = "cfa4cf1d-a337-4481-aa99-19d8f3d63f7c";
metadataList.add(metadata3);
KeyValuePair metadata4 = new KeyValuePair();
metadata4.name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name";
metadata4.value = "General";
metadataList.add(metadata4);
KeyValuePair metadata5 = new KeyValuePair();
metadata5.name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits";
metadata5.value = "0";
metadataList.add(metadata5);
KeyValuePair metadata6 = new KeyValuePair();
metadata6.name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId";
metadata6.value = "00000000-0000-0000-0000-000000000000";
metadataList.add(metadata6);
contentInfo.metadata = metadataList;

LabelingOptions labelingOptions = new LabelingOptions();
labelingOptions.additionalDataManager().put("assignmentMethod@odata.type", new JsonPrimitive("#microsoft.graph.assignmentMethod"));
labelingOptions.assignmentMethod = AssignmentMethod.STANDARD;
labelingOptions.additionalDataManager().put("labelId@odata.type", new JsonPrimitive("#Guid"));
labelingOptions.labelId = UUID.fromString("97309856-9c28-4ac6-9382-5f8bc20c457b");
labelingOptions.downgradeJustification = null;
labelingOptions.additionalDataManager().put("extendedProperties@odata.type", new JsonPrimitive("#Collection(microsoft.graph.keyValuePair)"));
LinkedList<KeyValuePair> extendedPropertiesList = new LinkedList<KeyValuePair>();
labelingOptions.extendedProperties = extendedPropertiesList;

graphClient.informationProtection().policy().labels()
    .evaluateApplication(InformationProtectionLabelEvaluateApplicationParameterSet
        .newBuilder()
        .withContentInfo(contentInfo)
        .withLabelingOptions(labelingOptions)
        .build())
    .buildRequest( requestOptions )
    .post();

```