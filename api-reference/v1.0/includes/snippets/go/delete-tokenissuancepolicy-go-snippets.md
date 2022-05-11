---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb54dec0e7b25d9c4eca4fb76299aee1f6ea2aa4
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326734"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tokenIssuancePolicyId := "tokenIssuancePolicy-id"
graphClient.Policies().TokenIssuancePoliciesById(&tokenIssuancePolicyId).Delete()


```