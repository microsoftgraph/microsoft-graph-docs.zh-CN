---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6129f3bcf5a312701aa858b02c6750621e6b7bad
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843812"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2xUserFlows["B2X_1_testuserflow"].PostAttributeCollection.Reference
    .Request()
    .PutAsync("{id}");

```