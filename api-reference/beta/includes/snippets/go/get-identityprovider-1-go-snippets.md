---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8be25c53934cb84b2170d108a7ccb33b2c5d2e96
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083237"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

identityProviderId := "identityProvider-id"
result, err := graphClient.IdentityProvidersById(&identityProviderId).Get(options)


```