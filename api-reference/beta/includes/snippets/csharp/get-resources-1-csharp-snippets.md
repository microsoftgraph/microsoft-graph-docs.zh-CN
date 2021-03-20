---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0f37de388df4cba34a2ac3edc8dc95f7c578e83
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951793"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var resources = await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Resources
    .Request()
    .GetAsync();

```