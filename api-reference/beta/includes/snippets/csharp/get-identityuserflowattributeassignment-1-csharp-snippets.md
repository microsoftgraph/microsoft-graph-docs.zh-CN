---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a403a0aceea64bc3dfb9d897ac92648b98cfe29dd5063edd1dd1e6abf8d6aad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161940"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userAttributeAssignments = await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].UserAttributeAssignments
    .Request()
    .GetAsync();

```