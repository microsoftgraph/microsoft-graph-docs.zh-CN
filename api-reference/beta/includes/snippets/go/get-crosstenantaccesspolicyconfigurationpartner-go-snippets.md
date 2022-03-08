---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0667fbc2eebfbfc4727a6e7355f0fe7bdb6b8794
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335743"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

crossTenantAccessPolicyConfigurationPartnerTenantId := "crossTenantAccessPolicyConfigurationPartner-tenantId"
result, err := graphClient.Policies().CrossTenantAccessPolicy().PartnersById(&crossTenantAccessPolicyConfigurationPartnerTenantId).Get(nil)


```