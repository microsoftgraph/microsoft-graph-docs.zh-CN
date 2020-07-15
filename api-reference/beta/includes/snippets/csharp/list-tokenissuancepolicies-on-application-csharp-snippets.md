---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6dd7eb02e15c79e8b65c2d442d70dc3f5cef554c
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142242"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenIssuancePolicies = await graphClient.Applications["{id}"].TokenIssuancePolicies
    .Request()
    .GetAsync();

```