---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 269ded5469caf2ad54d213a74954ce9c7ffc59770996dccd763c5db2d7668104
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161415"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contentInfo = new ContentInfo
{
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
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"format@odata.type", "#microsoft.graph.contentFormat"},
        {"state@odata.type", "#microsoft.graph.contentState"},
        {"metadata@odata.type", "#Collection(microsoft.graph.keyValuePair)"}
    }
};

var labelingOptions = new LabelingOptions
{
    AssignmentMethod = AssignmentMethod.Standard,
    LabelId = Guid.Parse("97309856-9c28-4ac6-9382-5f8bc20c457b"),
    DowngradeJustification = null,
    ExtendedProperties = new List<KeyValuePair>()
    {
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"assignmentMethod@odata.type", "#microsoft.graph.assignmentMethod"},
        {"labelId@odata.type", "#Guid"},
        {"extendedProperties@odata.type", "#Collection(microsoft.graph.keyValuePair)"}
    }
};

await graphClient.InformationProtection.Policy.Labels
    .EvaluateApplication(contentInfo,labelingOptions)
    .Request()
    .Header("User-Agent","ContosoLOBApp/1.0")
    .PostAsync();

```