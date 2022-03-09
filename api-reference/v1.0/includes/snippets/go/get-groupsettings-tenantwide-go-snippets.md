---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 570f9ef37c599add7c140fb797ae8e786796ad5f
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393541"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupSettingId := "groupSetting-id"
result, err := graphClient.GroupSettingsById(&groupSettingId).Get(nil)


```