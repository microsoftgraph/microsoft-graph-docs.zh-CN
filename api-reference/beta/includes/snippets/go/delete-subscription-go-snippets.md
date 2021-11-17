---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6c69951db5d837b9cb6bdb8a44c3b1cf9ae20208
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61033738"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

subscriptionId := "subscription-id"
graphClient.SubscriptionsById(&subscriptionId).Delete(options)


```