---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83e6ae821c5cbe5e717e38c6d02d8ab0e62686cb
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412303"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

servicePrincipalId := "servicePrincipal-id"
synchronizationJobId := "synchronizationJob-id"
directoryDefinitionId := "directoryDefinition-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).Synchronization().JobsById(&synchronizationJobId).Schema().DirectoriesById(&directoryDefinitionId).Discover(servicePrincipal-id, synchronizationJob-id, directoryDefinition-id).Post(nil)


```