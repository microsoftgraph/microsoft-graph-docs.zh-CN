---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 317ea850ce60b01793113e00b3b92e3b1d2492bc
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843833"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2xUserFlows["B2X_1_testuserflow"].PostFederationSignup.Reference
    .Request()
    .PutAsync("{id}");

```