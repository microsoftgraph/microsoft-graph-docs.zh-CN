---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d81e85f91edd75ffa8d91c462f9e585b64d6f656
ms.sourcegitcommit: 6deec57c0ab736260ee3599703bfd3f567ee6d82
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2019
ms.locfileid: "37045332"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = await graphClient.Me.Messages["AAMkAGUzY5QKjAAA="].Attachments["AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8="]
    .Request()
    .GetAsync();

```