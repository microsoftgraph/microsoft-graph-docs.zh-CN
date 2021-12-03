---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a49d4b1ca4446e86022cde7e4e2a78578e42535
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288547"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
graphClient.UsersById(&userId).Delete(nil)


```