---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eed6eb481adb64e094d77f1cc86bb7c17675515c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348299"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamworkDeviceId := "teamworkDevice-id"
teamworkDeviceOperationId := "teamworkDeviceOperation-id"
result, err := graphClient.Teamwork().DevicesById(&teamworkDeviceId).OperationsById(&teamworkDeviceOperationId).Get(nil)


```