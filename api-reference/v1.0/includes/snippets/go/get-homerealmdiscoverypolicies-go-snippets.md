---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd9644e6bdff258bb2a028e2e90ed7a93a71daf9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087061"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Policies().HomeRealmDiscoveryPolicies().Get(options)


```