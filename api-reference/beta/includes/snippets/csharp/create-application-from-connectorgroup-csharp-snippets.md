---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74d469a3dd8b844e7d335f5fd99a84f98a8fe608
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796751"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{application-id}"].ConnectorGroup.Reference
    .Request()
    .PutAsync("{id}");

```