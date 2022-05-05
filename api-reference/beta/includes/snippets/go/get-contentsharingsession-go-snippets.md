---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4237755a9562d8e5b0ec40d7ad08c23497b008b
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210363"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

callId := "call-id"
contentSharingSessionId := "contentSharingSession-id"
result, err := graphClient.Communications().CallsById(&callId).ContentSharingSessionsById(&contentSharingSessionId).Get(nil)


```