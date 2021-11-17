---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fbb9f4910672d50233ee1edb5b67ec5b71c5996
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61012969"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

servicePrincipalId := "servicePrincipal-id"
delegatedPermissionClassificationId := "delegatedPermissionClassification-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).DelegatedPermissionClassificationsById(&delegatedPermissionClassificationId).Delete(options)


```