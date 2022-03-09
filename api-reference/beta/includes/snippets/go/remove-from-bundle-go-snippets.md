---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cbb728c7587aded6cc6758fad338f062258d9655
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395179"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

driveItemId := "driveItem-id"
driveItemId1 := "driveItem-id1"
graphClient.Drive().BundlesById(&driveItemId).ChildrenById(&driveItemId1).Delete(nil)


```