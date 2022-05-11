---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88812d07283d311c221e6ffcb0cea76d83403d8c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326630"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupSettingId := "groupSetting-id"
graphClient.GroupSettingsById(&groupSettingId).Delete()


```