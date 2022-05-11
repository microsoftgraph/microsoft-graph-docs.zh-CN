---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf1cf60c09a3324b12eabc092fa67e176f665a98
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329256"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamworkDeviceId := "teamworkDevice-id"
teamworkDeviceOperationId := "teamworkDeviceOperation-id"
result, err := graphClient.Teamwork().DevicesById(&teamworkDeviceId).OperationsById(&teamworkDeviceOperationId).Get()


```