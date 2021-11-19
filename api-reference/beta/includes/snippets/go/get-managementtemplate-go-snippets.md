---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 439c2557a09604a7a4d1827fa53e21a84fbb121e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092184"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

managementTemplateId := "managementTemplate-id"
result, err := graphClient.TenantRelationships().ManagedTenants().ManagementTemplatesById(&managementTemplateId).Get(options)


```