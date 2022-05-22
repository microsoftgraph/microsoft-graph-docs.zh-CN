---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3786e287115443bece14d99ff86d841a96fdb12e
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65628891"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAgreementFileLocalization()
fileName := "Contoso ToU for guest users (French)"
requestBody.SetFileName(&fileName)
language := "fr-FR"
requestBody.SetLanguage(&language)
isDefault := false
requestBody.SetIsDefault(&isDefault)
isMajorVersion := false
requestBody.SetIsMajorVersion(&isMajorVersion)
displayName := "Contoso ToU for guest users (French)"
requestBody.SetDisplayName(&displayName)
fileData := msgraphsdk.NewAgreementFileData()
requestBody.SetFileData(fileData)
data := []byte("base64JVBERi0xLjUKJb/3ov4KNCAwIG9iago8PCAvTGluZWFyaX//truncated-binary-data")
fileData.SetData(&data)
agreementId := "agreement-id"
result, err := graphClient.IdentityGovernance().TermsOfUse().AgreementsById(&agreementId).Files().Post(requestBody)


```