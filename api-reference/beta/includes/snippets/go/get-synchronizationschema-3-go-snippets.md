---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5dbeeddf3c0551f773ed0de99294fb9740811b87
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326548"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

headers := map[string]string{
    "Authorization": "Bearer {Token}"
}
options := &msgraphsdk.SchemaRequestBuilderGetRequestConfiguration{
    Headers: headers,
}
servicePrincipalId := "servicePrincipal-id"
synchronizationJobId := "synchronizationJob-id"
result, err := graphClient.ServicePrincipalsById(&servicePrincipalId).Synchronization().JobsById(&synchronizationJobId).Schema().GetWithRequestConfigurationAndResponseHandler(options, nil)


```