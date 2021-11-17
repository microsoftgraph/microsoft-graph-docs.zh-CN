---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ecba3c2d799d54316e564f724e66ad4b2b0bbcfb
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61017253"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

trustFrameworkKeySetId := "trustFrameworkKeySet-id"
graphClient.TrustFramework().KeySetsById(&trustFrameworkKeySetId).Delete(options)


```