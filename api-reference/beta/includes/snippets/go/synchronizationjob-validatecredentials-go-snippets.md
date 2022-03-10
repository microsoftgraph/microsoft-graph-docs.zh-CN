---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f51fc347128edd92d93615fb4731d0a2c152ac6c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412745"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

servicePrincipalId := "servicePrincipal-id"
synchronizationJobId := "synchronizationJob-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).Synchronization().JobsById(&synchronizationJobId).ValidateCredentials(servicePrincipal-id, synchronizationJob-id).Post(nil)


```