---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2dbac1c4548c69c33252d7e3442cae2addc47f88
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60981153"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.TenantRelationships().ManagedTenants().ConditionalAccessPolicyCoverages().Get(options)


```