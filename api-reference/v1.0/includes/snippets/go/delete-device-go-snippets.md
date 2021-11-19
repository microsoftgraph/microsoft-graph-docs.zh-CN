---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6703956c2d5d5f34c0bd0a94f2c3e72fcb6d502a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093502"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

deviceId := "device-id"
graphClient.DevicesById(&deviceId).Delete(options)


```