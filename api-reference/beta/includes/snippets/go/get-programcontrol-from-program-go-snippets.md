---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fefd93c9aeb88e2a1b3ffe031b838ec07ba41c20
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091933"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

programId := "program-id"
result, err := graphClient.ProgramsById(&programId).Controls().Get(options)


```