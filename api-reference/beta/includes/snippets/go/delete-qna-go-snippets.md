---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6858f10739b0c34ede3bb75dc8380bd22224b40
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412660"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

qnaId := "qna-id"
result, err := graphClient.Search().QnasById(&qnaId).Delete(nil)


```