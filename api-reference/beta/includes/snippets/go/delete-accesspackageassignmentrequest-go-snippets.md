---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ec9208310f927c73068dc4706912a83963235c6
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090837"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageAssignmentRequestId := "accessPackageAssignmentRequest-id"
graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentRequestsById(&accessPackageAssignmentRequestId).Delete(options)


```