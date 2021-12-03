---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7645d57d519af38b84ae3b9276221612cb4bf49a
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61289175"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

programId := "program-id"
graphClient.ProgramsById(&programId).Delete(nil)


```