---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82630611ce8630dcf4b8137f9ba50402d908f0bd
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328622"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
userAccountType := "administrator"
requestBody.SetUserAccountType(&userAccountType)
osVersion := "windows10"
requestBody.SetOsVersion(&osVersion)
cloudPCId := "cloudPC-id"
graphClient.DeviceManagement().VirtualEndpoint().CloudPCsById(&cloudPCId).Reprovision(cloudPC-id).Post(requestBody)


```