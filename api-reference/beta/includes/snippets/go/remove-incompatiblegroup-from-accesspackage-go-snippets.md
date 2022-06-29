---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f58222af18c19363e105d590b363ac3c7b9cbee1
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65693922"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageId := "accessPackage-id"
groupId := "group-id"
graphClient.IdentityGovernance().EntitlementManagement().AccessPackagesById(&accessPackageId).IncompatibleGroupsById(&groupId).$ref().Delete()


```