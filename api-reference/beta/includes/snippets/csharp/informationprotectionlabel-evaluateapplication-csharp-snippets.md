---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43669b398e2b9c1bb69841d20d9eb9abd10e7842
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994438"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contentInfo = new ContentInfo
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"metadata@odata.type","#Collection(microsoft.graph.keyValuePair)"},
        {"state@odata.type","#microsoft.graph.contentState"},
        {"format@odata.type","#microsoft.graph.contentFormat"}
    },
    Format = ContentFormat.Default,
    Identifier = null,
    State = ContentState.Rest,
    Metadata = new List<KeyValuePair>()
    {
        new KeyValuePair
        {
            Name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled",
            Value = "True"
        },
        new KeyValuePair
        {
            Name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method",
            Value = "Standard"
        },
        new KeyValuePair
        {
            Name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate",
            Value = "1/1/0001 12:00:00 AM"
        },
        new KeyValuePair
        {
            Name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId",
            Value = "cfa4cf1d-a337-4481-aa99-19d8f3d63f7c"
        },
        new KeyValuePair
        {
            Name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name",
            Value = "General"
        },
        new KeyValuePair
        {
            Name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits",
            Value = "0"
        },
        new KeyValuePair
        {
            Name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId",
            Value = "00000000-0000-0000-0000-000000000000"
        }
    }
};

var labelingOptions = new LabelingOptions
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"extendedProperties@odata.type","#Collection(microsoft.graph.keyValuePair)"},
        {"labelId@odata.type","#Guid"},
        {"assignmentMethod@odata.type","#microsoft.graph.assignmentMethod"}
    },
    AssignmentMethod = AssignmentMethod.Standard,
    LabelId = Guid.Parse("97309856-9c28-4ac6-9382-5f8bc20c457b"),
    DowngradeJustification = null,
    ExtendedProperties = new List<KeyValuePair>()
    {
    }
};

await graphClient.Informationprotection.Policy.Labels
    .EvaluateApplication(contentInfo,labelingOptions)
    .Request()
    .PostAsync();

```