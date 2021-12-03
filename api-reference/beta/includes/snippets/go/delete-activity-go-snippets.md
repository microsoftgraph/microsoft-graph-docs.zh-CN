---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a667ecf128464b14db86739eb258042430bb39dd
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61289187"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userActivityId := "userActivity-id"
graphClient.Me().ActivitiesById(&userActivityId).Delete(nil)


```