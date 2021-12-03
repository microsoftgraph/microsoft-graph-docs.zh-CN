---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea37fc659f7d571ab80a835f7f588d7b80b97ce4
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287822"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

directoryObjectId := "directoryObject-id"
graphClient.DirectoryObjectsById(&directoryObjectId).Delete(nil)


```