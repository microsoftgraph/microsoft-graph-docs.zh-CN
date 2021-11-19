---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8dd2af69392b4e709402a241dae8daadf9a69ef8
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089717"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

headers := map[string]string{
    "Accept-Language": "fr-FR"
}
options := &msgraphsdk.BrandingRequestBuilderGetOptions{
    H: headers,
}
organizationId := "organization-id"
result, err := graphClient.OrganizationById(&organizationId).Branding().Get(options)


```