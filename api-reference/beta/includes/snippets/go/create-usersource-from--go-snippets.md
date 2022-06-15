---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79abb80e6f43d911f8a6054e1a4963d5f8f29fc6
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095165"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUserSource()
email := "admin@M365x809305.onmicrosoft.com"
requestBody.SetEmail(&email)
includedSources := "mailbox, site"
requestBody.SetIncludedSources(&includedSources)
ediscoveryCaseId := "ediscoveryCase-id"
ediscoveryCustodianId := "ediscoveryCustodian-id"
result, err := graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).CustodiansById(&ediscoveryCustodianId).UserSources().Post(requestBody)


```