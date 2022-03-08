---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a63ba4f62defb2a70c2c8671034f4ef1e388edd3
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338909"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

qnaId := "qna-id"
graphClient.Search().QnasById(&qnaId).Delete(nil)


```