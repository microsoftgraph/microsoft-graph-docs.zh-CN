---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ddc47e4f64589653c8a266a0c8e24bfaa6d26150
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137753"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.PrivilegedRoleAssignmentRequests().My()().Get(nil)


```