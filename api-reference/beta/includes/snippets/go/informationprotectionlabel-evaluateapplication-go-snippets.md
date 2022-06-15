---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8247d44ee273b7a99eefb80846d07d57e477166a
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098682"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
contentInfo := msgraphsdk.NewContentInfo()
requestBody.SetContentInfo(contentInfo)
format := "default"
contentInfo.SetFormat(&format)
contentInfo.SetIdentifier(nil)
state := "rest"
contentInfo.SetState(&state)
contentInfo.SetMetadata( []KeyValuePair {
    msgraphsdk.NewKeyValuePair(),
name := "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled"
    SetName(&name)
value := "True"
    SetValue(&value)
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.keyValuePair",
    }
    msgraphsdk.NewKeyValuePair(),
name := "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method"
    SetName(&name)
value := "Standard"
    SetValue(&value)
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.keyValuePair",
    }
    msgraphsdk.NewKeyValuePair(),
name := "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate"
    SetName(&name)
value := "1/1/0001 12:00:00 AM"
    SetValue(&value)
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.keyValuePair",
    }
    msgraphsdk.NewKeyValuePair(),
name := "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId"
    SetName(&name)
value := "cfa4cf1d-a337-4481-aa99-19d8f3d63f7c"
    SetValue(&value)
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.keyValuePair",
    }
    msgraphsdk.NewKeyValuePair(),
name := "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name"
    SetName(&name)
value := "General"
    SetValue(&value)
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.keyValuePair",
    }
    msgraphsdk.NewKeyValuePair(),
name := "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits"
    SetName(&name)
value := "0"
    SetValue(&value)
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.keyValuePair",
    }
    msgraphsdk.NewKeyValuePair(),
name := "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId"
    SetName(&name)
value := "00000000-0000-0000-0000-000000000000"
    SetValue(&value)
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.keyValuePair",
    }
}
contentInfo.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.contentInfo",
    "format@odata.type": "#microsoft.graph.contentFormat",
    "state@odata.type": "#microsoft.graph.contentState",
    "metadata@odata.type": "#Collection(microsoft.graph.keyValuePair)",
}
labelingOptions := msgraphsdk.NewLabelingOptions()
requestBody.SetLabelingOptions(labelingOptions)
assignmentMethod := "standard"
labelingOptions.SetAssignmentMethod(&assignmentMethod)
labelId := "97309856-9c28-4ac6-9382-5f8bc20c457b"
labelingOptions.SetLabelId(&labelId)
labelingOptions.SetDowngradeJustification(nil)
labelingOptions.SetExtendedProperties( []KeyValuePair {
}
labelingOptions.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.labelingOptions",
    "assignmentMethod@odata.type": "#microsoft.graph.assignmentMethod",
    "labelId@odata.type": "#Guid",
    "extendedProperties@odata.type": "#Collection(microsoft.graph.keyValuePair)",
}
headers := map[string]string{
    "User-Agent": "ContosoLOBApp/1.0"
}
options := &msgraphsdk.EvaluateApplicationRequestBuilderPostRequestConfiguration{
    Headers: headers,
}
result, err := graphClient.InformationProtection().Policy().Labels().EvaluateApplication().PostWithRequestConfigurationAndResponseHandler(requestBody, options, nil)


```