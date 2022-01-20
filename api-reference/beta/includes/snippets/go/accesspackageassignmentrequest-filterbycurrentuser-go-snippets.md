---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: daa40a4bcca8cb916586279ee089953e77ff6b26
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62107207"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageAssignmentRequestId := "accessPackageAssignmentRequest-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentRequestsById(&accessPackageAssignmentRequestId).Get(nil)


```