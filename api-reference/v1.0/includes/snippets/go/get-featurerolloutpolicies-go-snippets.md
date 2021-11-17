---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dbbadc8fdfc6004d581aa662f133cf9532a05095
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60984723"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Policies().FeatureRolloutPolicies().Get(options)


```