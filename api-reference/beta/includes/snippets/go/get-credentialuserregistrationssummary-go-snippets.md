---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f48eb7e350136b2a75defddcbf2b576f337f379f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61002917"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

credentialUserRegistrationsSummaryId := "credentialUserRegistrationsSummary-id"
result, err := graphClient.TenantRelationships().ManagedTenants().CredentialUserRegistrationsSummariesById(&credentialUserRegistrationsSummaryId).Get(options)


```