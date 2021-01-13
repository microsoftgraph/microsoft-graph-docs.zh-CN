---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a048dccee65d02ba6c35ccd01d86cc2a91d1cf3
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844014"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2cUserFlows["B2C_1_testuserflow"].PostFederationSignup.Reference
    .Request()
    .PutAsync("{id}");

```