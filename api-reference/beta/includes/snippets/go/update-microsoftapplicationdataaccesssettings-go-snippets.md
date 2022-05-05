---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3dc8c4f33bbaaaad620a8cfdaecbbda94d44238
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212427"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMicrosoftApplicationDataAccessSettings()
disabledForGroup := "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
requestBody.SetDisabledForGroup(&disabledForGroup)
options := &msgraphsdk.MicrosoftApplicationDataAccessRequestBuilderPatchOptions{
    Body: requestBody,
}
organizationId := "organization-id"
graphClient.OrganizationById(&organizationId).Settings().MicrosoftApplicationDataAccess().Patch(options)


```