---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26c210160b1cf4376e0657fc8f16cc4514285a46
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61021291"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Security().SecureScoreControlProfiles().Get(options)


```