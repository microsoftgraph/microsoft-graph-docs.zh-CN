---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 970b2dce6bf0982e3a69fc112895e7fb23de6a51
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288992"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

subscriptionId := "subscription-id"
graphClient.SubscriptionsById(&subscriptionId).Delete(nil)


```