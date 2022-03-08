---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5a520906306d012582ce2d0e764dd2ba80e0983
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338267"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

qnaId := "qna-id"
result, err := graphClient.Search().QnasById(&qnaId).Get(nil)


```