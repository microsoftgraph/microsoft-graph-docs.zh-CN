---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f10941af730c277a70d43364b29e9861fc704978f0c2e4ce179d4b578111c972
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161938"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userAttributeAssignments = await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].UserAttributeAssignments
    .Request()
    .Expand("userAttribute")
    .GetAsync();

```