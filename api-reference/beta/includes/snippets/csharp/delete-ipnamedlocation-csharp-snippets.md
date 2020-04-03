---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae63e4b2ca3fb23082e2f2fcd656f1f180c48541
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43127220"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.ConditionalAccess.NamedLocations["0854951d-5fc0-4eb1-b392-9b2c9d7949c2"]
    .Request()
    .DeleteAsync();

```