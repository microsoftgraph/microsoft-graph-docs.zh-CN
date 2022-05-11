---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f86833f21a7fcbe34ede67e17f3ba513942807a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329062"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

driveItemId := "driveItem-id"
graphClient.Drive().ItemsById(&driveItemId).Delete()


```