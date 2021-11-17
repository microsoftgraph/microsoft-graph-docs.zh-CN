---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36906b72f3bfbba836a213d316d5f313fcab9cac
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61007328"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.RoleManagement().EntitlementManagement().RoleDefinitions().Get(options)


```