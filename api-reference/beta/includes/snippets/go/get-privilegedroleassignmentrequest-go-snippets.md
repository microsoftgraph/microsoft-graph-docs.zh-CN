---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f9b3b20fdaa4c4a6b367693f729c0f5d2c556f2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023678"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.PrivilegedRoleAssignmentRequests().Get(options)


```