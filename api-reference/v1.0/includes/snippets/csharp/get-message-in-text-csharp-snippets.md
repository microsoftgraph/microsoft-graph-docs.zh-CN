---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95e85aa64ed3c6ac610e0fe46ffe158e8db5fbb8
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44685031"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["AAMkAGI1AAAoZCfHAAA="]
    .Request()
    .Header("Prefer","outlook.body-content-type=\"text\"")
    .Select("subject,body,bodyPreview,uniqueBody")
    .GetAsync();

```