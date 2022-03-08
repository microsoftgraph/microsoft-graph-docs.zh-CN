---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7128395a197023f99cea4e2b7b9f5a51c21be1ea
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335785"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

crossTenantAccessPolicyConfigurationPartnerTenantId := "crossTenantAccessPolicyConfigurationPartner-tenantId"
graphClient.Policies().CrossTenantAccessPolicy().PartnersById(&crossTenantAccessPolicyConfigurationPartnerTenantId).Delete(nil)


```