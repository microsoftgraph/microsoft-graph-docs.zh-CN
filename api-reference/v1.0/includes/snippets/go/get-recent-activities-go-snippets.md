---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d3f5c6b9e66181e02ce494bc4f86643ecf084b7
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287659"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userActivityId := "userActivity-id"
result, err := graphClient.Me().ActivitiesById(&userActivityId).Get(nil)


```