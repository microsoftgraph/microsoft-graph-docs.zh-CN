---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 11c14dbaaaa281485c73c516047ee922dfd2fd41
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903505"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{id}"].Owners["{id}"].Reference
    .Request()
    .DeleteAsync();

```