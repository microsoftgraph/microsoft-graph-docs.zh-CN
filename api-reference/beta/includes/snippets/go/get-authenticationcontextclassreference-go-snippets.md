---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97a509ba48481b0ba6331e3c23234d157771b2bb
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348781"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

authenticationContextClassReferenceId := "authenticationContextClassReference-id"
result, err := graphClient.Identity().ConditionalAccess().AuthenticationContextClassReferencesById(&authenticationContextClassReferenceId).Get(nil)


```