---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e8142b1094a180b2e3196ef579cd46c3f3fa6be
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904115"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.UserFlowAttributes["{id}"]
    .Request()
    .DeleteAsync();

```