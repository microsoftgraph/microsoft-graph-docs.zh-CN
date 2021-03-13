---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb711e2c8b6b16e9c94e46468ea0489312a8a3e9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800602"
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

await graphClient.Communications.Calls["{call-id}"]
    .Answer(callbackUri,mediaConfig,acceptedModalities,null)
    .Request()
    .PostAsync();

```