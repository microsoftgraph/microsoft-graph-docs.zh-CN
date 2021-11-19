---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ef2365137ed532a6f6378d642d463743f485140
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096879"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

servicePrincipalId := "servicePrincipal-id"
delegatedPermissionClassificationId := "delegatedPermissionClassification-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).DelegatedPermissionClassificationsById(&delegatedPermissionClassificationId).Delete(options)


```