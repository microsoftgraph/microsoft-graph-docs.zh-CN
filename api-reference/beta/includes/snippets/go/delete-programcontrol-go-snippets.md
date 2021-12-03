---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e43ed0cb67e2f2cf4aa0587df6c3053801742309
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288616"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

programControlId := "programControl-id"
graphClient.ProgramControlsById(&programControlId).Delete(nil)


```