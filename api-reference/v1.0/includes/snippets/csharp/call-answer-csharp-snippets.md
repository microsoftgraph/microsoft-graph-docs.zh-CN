---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f91c9f0f767ce046c433aaa2afd2d91930119635
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871135"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var callbackUri = "callbackUri-value";

var mediaConfig = new AppHostedMediaConfig
{
    Blob = "<Media Session Configuration Blob>"
};

var acceptedModalities = new List<Modality>()
{
    Modality.Audio
};

await graphClient.Communications.Calls["{id}"]
    .Answer(callbackUri,mediaConfig,acceptedModalities)
    .Request()
    .PostAsync();

```