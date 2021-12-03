---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a23d5955ebefd66863953176b5a2f38536efd4a
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288139"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

driveId := "drive-id"
result, err := graphClient.DrivesById(&driveId).Get(nil)


```