---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72ce5326acdfc0390abc12bd54bb0b2d14d27cdf
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871134"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var callbackUri = "https://bot.contoso.com/api/calls";

var acceptedModalities = new List<Modality>()
{
    Modality.Audio
};

var mediaConfig = new AppHostedMediaConfig
{
    Blob = "<Media Session Configuration Blob>"
};

await graphClient.Communications.Calls["57DAB8B1894C409AB240BD8BEAE78896"]
    .Answer(callbackUri,mediaConfig,acceptedModalities)
    .Request()
    .PostAsync();

```