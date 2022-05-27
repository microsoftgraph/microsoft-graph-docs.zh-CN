---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d5474c226f7d7bfcdaaac7dfec935abb2dad0dd
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65695291"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

applicationId := "application-id"
tokenLifetimePolicyId := "tokenLifetimePolicy-id"
graphClient.ApplicationsById(&applicationId).TokenLifetimePoliciesById(&tokenLifetimePolicyId).$ref().Delete()


```