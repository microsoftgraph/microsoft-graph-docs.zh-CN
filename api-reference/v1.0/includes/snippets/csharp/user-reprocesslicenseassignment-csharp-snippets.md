---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1762a4f7d8058ce66e5cea2d370921e3749318dd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798045"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"]
    .ReprocessLicenseAssignment()
    .Request()
    .PostAsync();

```