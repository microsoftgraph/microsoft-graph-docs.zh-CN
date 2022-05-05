---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b63134871643e93cf89fd21f33ec24c687fa0e5
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211612"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

callId := "call-id"
result, err := graphClient.Communications().CallsById(&callId).ContentSharingSessions().Get(nil)


```