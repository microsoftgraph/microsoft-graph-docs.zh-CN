---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b40a6e1946357426790a9337f71d8a7c9f7d771bfa31ce1a83b9b0cc9d305855
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105419"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].PostAttributeCollection.Reference
    .Request()
    .PutAsync("{id}");

```