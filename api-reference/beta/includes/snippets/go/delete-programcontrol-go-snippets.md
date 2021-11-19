---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d6a533918cb725c7049c43647f3cd05c83b2f02
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086893"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

programControlId := "programControl-id"
graphClient.ProgramControlsById(&programControlId).Delete(options)


```