---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05e0889a48d49ce2591d83fc7ae595f4c3271b1f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60994999"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Policies().AuthenticationMethodsPolicy().Get(options)


```