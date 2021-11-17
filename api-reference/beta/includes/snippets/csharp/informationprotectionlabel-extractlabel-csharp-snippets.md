---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3643e9d3423df510302f5166d97c906e22b238406ecbe5b961f8ea4a573c581e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278464"
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
            Value = "Top Secret"
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

await graphClient.InformationProtection.Policy.Labels
    .ExtractLabel(contentInfo)
    .Request()
    .Header("User-Agent","ContosoLOBApp/1.0")
    .PostAsync();

```