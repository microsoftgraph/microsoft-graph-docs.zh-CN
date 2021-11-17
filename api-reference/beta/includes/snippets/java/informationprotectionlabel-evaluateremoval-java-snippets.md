---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10044bc1567de26e172943a47371f7a837d5b1c1c6dcd6ea8bc6763b59548457
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278469"
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

DowngradeJustification downgradeJustification = new DowngradeJustification();
downgradeJustification.justificationMessage = "The information has been declassified.";
downgradeJustification.isDowngradeJustified = true;

graphClient.informationProtection().policy().labels()
    .evaluateRemoval(InformationProtectionLabelEvaluateRemovalParameterSet
        .newBuilder()
        .withContentInfo(contentInfo)
        .withDowngradeJustification(downgradeJustification)
        .build())
    .buildRequest( requestOptions )
    .post();

```