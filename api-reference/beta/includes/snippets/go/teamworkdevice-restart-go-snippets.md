---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a232324f87602636d9c86f76795850a1974fe02b
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412743"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamworkDeviceId := "teamworkDevice-id"
graphClient.Teamwork().DevicesById(&teamworkDeviceId).Restart(teamworkDevice-id).Post(nil)


```