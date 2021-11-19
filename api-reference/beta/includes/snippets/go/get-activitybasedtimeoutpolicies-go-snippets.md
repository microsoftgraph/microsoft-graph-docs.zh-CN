---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d53779530e3b8d7a1f61856dac574f9168d1aaf6
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090798"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Policies().ActivityBasedTimeoutPolicies().Get(options)


```