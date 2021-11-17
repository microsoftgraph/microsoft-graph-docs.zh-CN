---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f0b4983831a1f58a02dd26f6c68f59eee0b9fe9
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60994915"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
result, err := graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).IdentityProviders().Get(options)


```