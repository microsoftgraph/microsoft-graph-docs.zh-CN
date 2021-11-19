---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c26b996f7fc4b9f3b0e57dfea32d0fd75dcad190
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085144"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

trustFrameworkKeySetId := "trustFrameworkKeySet-id"
graphClient.TrustFramework().KeySetsById(&trustFrameworkKeySetId).Delete(options)


```