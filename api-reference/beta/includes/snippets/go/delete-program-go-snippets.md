---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64400e85d6cdd0741732b524e3be4e6770f42e2b
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63396768"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

programId := "program-id"
result, err := graphClient.ProgramsById(&programId).Delete(nil)


```