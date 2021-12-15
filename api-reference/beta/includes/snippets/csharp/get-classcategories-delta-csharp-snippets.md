---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57e6131c98c941563a308094b171d36583d773a1
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525952"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationCategory = await graphClient.Education.Classes["{educationClass-id}"].AssignmentCategories["{educationCategory-id}"]
    .Request()
    .GetAsync();

```