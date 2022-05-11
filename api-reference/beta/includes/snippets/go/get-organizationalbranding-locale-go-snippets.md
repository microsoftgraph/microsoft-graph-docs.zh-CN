---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36879cbd4d42e5c50337b08f17e4e7aa14e91709
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326895"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

headers := map[string]string{
    "Accept-Language": "fr-FR"
}
options := &msgraphsdk.BrandingRequestBuilderGetRequestConfiguration{
    Headers: headers,
}
organizationId := "organization-id"
result, err := graphClient.OrganizationById(&organizationId).Branding().GetWithRequestConfigurationAndResponseHandler(options, nil)


```