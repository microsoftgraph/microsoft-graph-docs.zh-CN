---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21a05067838680c532cb88a18c1db7a231d999a0
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49530615"
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
    .Answer(callbackUri,mediaConfig,acceptedModalities,null)
    .Request()
    .PostAsync();

```