---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c56be5e04334258ec0a997896904010d1e2dcfd
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328994"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthoredNote()
content := msgraphsdk.NewItemBody()
requestBody.SetContent(content)
content := "String"
content.SetContent(&content)
contentType := "text"
content.SetContentType(&contentType)
subjectRightsRequestId := "subjectRightsRequest-id"
result, err := graphClient.Privacy().SubjectRightsRequestsById(&subjectRightsRequestId).Notes().Post(requestBody)


```