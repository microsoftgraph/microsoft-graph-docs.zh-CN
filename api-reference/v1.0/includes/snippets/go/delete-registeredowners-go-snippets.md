---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab86721bff645ee87829d287443d2103eac36c4c
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65693768"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

deviceId := "device-id"
directoryObjectId := "directoryObject-id"
graphClient.DevicesById(&deviceId).RegisteredOwnersById(&directoryObjectId).$ref().Delete()


```