---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f7ac41024ed7a3103399d0a3623975f82408016
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328908"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamworkDeviceId := "teamworkDevice-id"
result, err := graphClient.Teamwork().DevicesById(&teamworkDeviceId).Configuration().Get()


```