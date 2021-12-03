---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1d42522bf621ec00140699cd88613f28e5f3269
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288097"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationalActivityId := "educationalActivity-id"
result, err := graphClient.Me().Profile().EducationalActivitiesById(&educationalActivityId).Get(nil)


```