---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1bd15e4f6d0fa65843dee7d32950885bb3ba45e6
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328745"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

directorySettingId := "directorySetting-id"
result, err := graphClient.SettingsById(&directorySettingId).Get()


```