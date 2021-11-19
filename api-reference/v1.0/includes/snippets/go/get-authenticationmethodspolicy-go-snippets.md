---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e83c84524a57af41c66c82f6c74e6233c6fd54a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086141"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Policies().AuthenticationMethodsPolicy().Get(options)


```