---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3782d4a2e78b1ef452534e2a889e4b2450213ac35019d8c18fb456ab2226582
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106046"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userAttributeAssignments = await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].UserAttributeAssignments
    .Request()
    .GetAsync();

```