---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef193ed8ca32c3628464f90f4dc10318baa1a361
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084252"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "LocalizedStrings":  []Object {
    }
}
options := &msgraphsdk.ContentRequestBuilderPutOptions{
    Body: requestBody,
}
b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
userFlowLanguageConfigurationId := "userFlowLanguageConfiguration-id"
userFlowLanguagePageId := "userFlowLanguagePage-id"
graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).LanguagesById(&userFlowLanguageConfigurationId).OverridesPagesById(&userFlowLanguagePageId).$value().Put(options)


```