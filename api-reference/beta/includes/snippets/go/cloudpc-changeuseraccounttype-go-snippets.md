---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e773ae021348583da890cea14e6566df93145c03
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326390"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUserAccountTypeRequestBody()
userAccountType := "administrator"
requestBody.SetUserAccountType(&userAccountType)
cloudPCId := "cloudPC-id"
graphClient.DeviceManagement().VirtualEndpoint().CloudPCsById(&cloudPCId).ChangeUserAccountType(cloudPC-id).Post(requestBody)


```