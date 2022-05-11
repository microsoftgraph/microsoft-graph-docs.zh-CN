---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 357092f70fdb5757705405665de0562a2542f819
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326770"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.RoleAssignmentsRequestBuilderGetQueryParameters{
    Filter%20: "%20principalIds/any(x:x%20eq%20'564ae70c-73d9-476b-820b-fb61eb7384b9')",
}
options := &msgraphsdk.RoleAssignmentsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.RoleManagement().DeviceManagement().RoleAssignments().GetWithRequestConfigurationAndResponseHandler(options, nil)


```