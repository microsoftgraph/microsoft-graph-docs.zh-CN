---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0b947cefe3dc98beb9a02825d2ec0cb51d7b891
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60984359"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Policies().PermissionGrantPolicies().Get(options)


```