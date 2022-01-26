---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 77a0f4d364a5a6a46f4423c4ebbef2aa2b0670ca
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62224764"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userRegistrationDetailsId := "userRegistrationDetails-id"
result, err := graphClient.Reports().AuthenticationMethods().UserRegistrationDetailsById(&userRegistrationDetailsId).Get(nil)


```