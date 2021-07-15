---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36f892fb974f1126d1a25bb73ca39d665497f821
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439745"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userFlowIdentityProviders = await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].UserFlowIdentityProviders
    .Request()
    .GetAsync();

```