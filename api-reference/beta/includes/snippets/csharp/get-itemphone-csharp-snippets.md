---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9fcb75e05c0e4d5e29cef79a625b3fcc559f71ec
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792704"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemPhone = await graphClient.Me.Profile.Phones["{itemPhone-id}"]
    .Request()
    .GetAsync();

```