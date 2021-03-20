---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6283bd31814fc2757df0c2907ce79a2525bb82a1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944537"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userAttributeAssignments = await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].UserAttributeAssignments
    .Request()
    .Expand("userAttribute")
    .GetAsync();

```