---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47ddd6ef0f82863141314d006031b649b367e1d0
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694700"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

b2cIdentityUserFlowId := "b2cIdentityUserFlow-id"
identityProviderId := "identityProvider-id"
graphClient.Identity().B2cUserFlowsById(&b2cIdentityUserFlowId).IdentityProvidersById(&identityProviderId).$ref().Delete()


```