---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 923e79ade2806012fa7aa77fb9d74fa825f7afe3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944740"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userAttributeAssignments = await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlow-id}"].UserAttributeAssignments
    .Request()
    .Expand("userAttribute")
    .GetAsync();

```