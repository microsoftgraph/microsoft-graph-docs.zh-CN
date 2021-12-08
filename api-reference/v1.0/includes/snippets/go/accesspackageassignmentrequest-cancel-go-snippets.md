---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb6b2b6b9a451a5ac6d51d6b7a14eaa5728a09ec
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61337934"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageAssignmentRequestId := "accessPackageAssignmentRequest-id"
graphClient.IdentityGovernance().EntitlementManagement().AssignmentRequestsById(&accessPackageAssignmentRequestId).Cancel().Post(nil)


```