---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9ce8c00cfee1c1aba30d08e838db7134691a18f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328300"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

deviceId := "device-id"
result, err := graphClient.DevicesById(&deviceId).MemberOf().Get()


```