---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03e3be2c2b7f1c34c2dd89259d78d60285599a8d
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903904"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityUserFlowAttribute = await graphClient.Identity.UserFlowAttributes["{id}"]
    .Request()
    .GetAsync();

```