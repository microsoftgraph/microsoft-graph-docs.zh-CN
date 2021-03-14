---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5145e65dc0467deabed1755889329ced7ed82b4f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810340"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Manager.Reference
    .Request()
    .PutAsync("{id}");

```