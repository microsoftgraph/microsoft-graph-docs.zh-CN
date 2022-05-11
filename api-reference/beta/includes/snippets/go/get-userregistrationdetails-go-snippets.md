---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd8bd90f8c2e9d7d2bf4c57a874797873ba64680
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328775"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userRegistrationDetailsId := "userRegistrationDetails-id"
result, err := graphClient.Reports().AuthenticationMethods().UserRegistrationDetailsById(&userRegistrationDetailsId).Get()


```