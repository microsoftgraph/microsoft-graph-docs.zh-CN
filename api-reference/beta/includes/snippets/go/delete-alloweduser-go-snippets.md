---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4a87b4e240146346f30e61dc1e77a82caa19000
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65693817"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

printerShareId := "printerShare-id"
userId := "user-id"
graphClient.Print().PrinterSharesById(&printerShareId).AllowedUsersById(&userId).$ref().Delete()


```