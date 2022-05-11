---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d4d23f5d6adfbb783c3750ccc5debbd3940dd5e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326058"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

driveId := "drive-id"
driveItemId := "driveItem-id"
result, err := graphClient.DrivesById(&driveId).ItemsById(&driveItemId).Analytics().Get()


```