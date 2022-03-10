---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8492c565b354ec94f23355e125e8ca6f9df939cf
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411946"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
result, err := graphClient.TermStore().GroupsById(&groupId).Delete(nil)


```