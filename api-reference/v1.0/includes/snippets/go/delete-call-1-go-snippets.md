---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47d7f1f5994ea4977787f0c78c1e6c53b4ca3588
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087181"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

callId := "call-id"
graphClient.Communications().CallsById(&callId).Delete(options)


```