---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef8b711a2f7bee18c4d2c1c4a0eda0cd94c77477
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905499"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipals = await graphClient.ServicePrincipals
    .Request()
    .GetAsync();

```