---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b65a2e2374e50a437a15198b388c3d0a0a14e188
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394248"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

applicationId := "application-id"
extensionPropertyId := "extensionProperty-id"
result, err := graphClient.ApplicationsById(&applicationId).ExtensionPropertiesById(&extensionPropertyId).Get(nil)


```