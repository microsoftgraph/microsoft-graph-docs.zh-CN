---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff440f45eb80b7bfa1682fc079832d12127fc0ea
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60981069"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.TenantRelationships().ManagedTenants().ManagementTemplates().Get(options)


```