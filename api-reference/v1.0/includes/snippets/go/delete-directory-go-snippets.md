---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd7cdb9f62d5c01e5862aece6712a1d981ceb746
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411634"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

directoryObjectId := "directoryObject-id"
result, err := graphClient.Directory().DeletedItemsById(&directoryObjectId).Delete(nil)


```