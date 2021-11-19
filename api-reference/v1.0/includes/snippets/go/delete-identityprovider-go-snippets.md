---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a085d96db0ec0a6350e4d65c08fbf48ea3c8e3e6
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103350"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

identityProviderId := "identityProvider-id"
graphClient.IdentityProvidersById(&identityProviderId).Delete(options)


```