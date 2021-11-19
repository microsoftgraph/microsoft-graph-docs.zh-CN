---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ff79c6f43e6a996d2f98dc095b49481fc6713d1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086187"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Me().Authentication().TemporaryAccessPassMethods().Get(options)


```