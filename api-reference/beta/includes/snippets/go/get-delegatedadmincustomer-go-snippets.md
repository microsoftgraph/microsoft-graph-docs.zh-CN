---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d159d0951f90ea3c2463a21f839fa7933b4a71e0
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202437"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

delegatedAdminCustomerId := "delegatedAdminCustomer-id"
result, err := graphClient.TenantRelationships().DelegatedAdminCustomersById(&delegatedAdminCustomerId).Get(nil)


```