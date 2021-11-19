---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5ec96ac58bfdf5d74f646a1a0fa51d0baeb3624
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092382"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.TrustFramework().Policies().Get(options)


```