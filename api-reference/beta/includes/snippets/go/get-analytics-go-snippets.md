---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8ca7a23f20916e5980db937c97b6b0d2c1f17f5
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393323"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

driveId := "drive-id"
driveItemId := "driveItem-id"
result, err := graphClient.DrivesById(&driveId).ItemsById(&driveItemId).Analytics().Get(nil)


```