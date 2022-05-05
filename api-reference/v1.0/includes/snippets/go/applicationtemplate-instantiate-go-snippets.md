---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c101713e72223e07b9aeb6397db435c315db8411
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220330"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDisplayNameRequestBody()
displayName := "Azure AD SAML Toolkit"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.InstantiateRequestBuilderPostOptions{
    Body: requestBody,
}
applicationTemplateId := "applicationTemplate-id"
result, err := graphClient.ApplicationTemplatesById(&applicationTemplateId).Instantiate(applicationTemplate-id).Post(options)


```