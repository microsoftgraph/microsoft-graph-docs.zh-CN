---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f454908ec99e5e72f5622176e836902f754b19bd
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60973766"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

servicePrincipalId := "servicePrincipal-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).Delete(options)


```