---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a0ba4e8f5ca01f5ffc98566f278c050b8dfc788
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327853"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

driveId := "drive-id"
result, err := graphClient.DrivesById(&driveId).Get()


```