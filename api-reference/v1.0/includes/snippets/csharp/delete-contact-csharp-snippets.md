---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa21dfc659a0ace31b07498a8a25f4f607c16dd1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793883"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Contacts["{contact-id}"]
    .Request()
    .DeleteAsync();

```