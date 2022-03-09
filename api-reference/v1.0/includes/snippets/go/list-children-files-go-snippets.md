---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4eee3a52471f52f1b830e375f2e795bc4d99596
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394969"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

driveId := "drive-id"
driveItemId := "driveItem-id"
result, err := graphClient.DrivesById(&driveId).ItemsById(&driveItemId).Children().Get(nil)


```