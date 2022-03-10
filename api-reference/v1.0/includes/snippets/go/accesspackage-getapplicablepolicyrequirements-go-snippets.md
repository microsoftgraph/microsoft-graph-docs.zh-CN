---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd7ec44d78eddb5fc96ac73244fb1282d4df5477
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411795"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageId := "accessPackage-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackagesById(&accessPackageId).GetApplicablePolicyRequirements(accessPackage-id).Post(nil)


```