---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a224b8520fe02f2b2aa5da717852a7ef5c1ac80
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080685"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organization = await graphClient.Organization["settings"]
    .Request()
    .GetAsync();

```