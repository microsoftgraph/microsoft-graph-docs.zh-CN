---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0fed471dff0c10d7fd74ad0371e28a3f23b6345
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287958"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

driveItemId := "driveItem-id"
graphClient.Drive().ItemsById(&driveItemId).Delete(nil)


```