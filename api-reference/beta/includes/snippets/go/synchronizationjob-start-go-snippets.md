---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b4e75b3a7a2eaf0721c4457528bb2e3af7de516
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412746"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

servicePrincipalId := "servicePrincipal-id"
synchronizationJobId := "synchronizationJob-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).Synchronization().JobsById(&synchronizationJobId).Start(servicePrincipal-id, synchronizationJob-id).Post(nil)


```