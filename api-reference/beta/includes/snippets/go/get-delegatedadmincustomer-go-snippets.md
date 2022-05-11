---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c23fbb216f67fef0b10d66d2323f028ca7131742
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327368"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

delegatedAdminCustomerId := "delegatedAdminCustomer-id"
result, err := graphClient.TenantRelationships().DelegatedAdminCustomersById(&delegatedAdminCustomerId).Get()


```