---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0fed471dff0c10d7fd74ad0371e28a3f23b6345
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758095"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

driveItemId := "driveItem-id"
graphClient.Drive().ItemsById(&driveItemId).Delete(nil)


```