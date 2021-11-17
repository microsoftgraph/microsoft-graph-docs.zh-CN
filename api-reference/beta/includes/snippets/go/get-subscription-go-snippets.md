---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c97f6109d7492a663a010a8278933e224c779cab
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61026114"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

subscriptionId := "subscription-id"
result, err := graphClient.SubscriptionsById(&subscriptionId).Get(options)


```