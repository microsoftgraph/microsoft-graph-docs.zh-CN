---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 110636686912496ac9f3315e36f1477415c868e7
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412108"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

servicePrincipalId := "servicePrincipal-id"
delegatedPermissionClassificationId := "delegatedPermissionClassification-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).DelegatedPermissionClassificationsById(&delegatedPermissionClassificationId).Delete(nil)


```