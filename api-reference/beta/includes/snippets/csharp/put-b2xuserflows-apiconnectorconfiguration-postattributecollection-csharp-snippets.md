---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f48696b7778a5bdfc20c317bb8f591879e1c9684
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799856"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].PostAttributeCollection.Reference
    .Request()
    .PutAsync("{id}");

```