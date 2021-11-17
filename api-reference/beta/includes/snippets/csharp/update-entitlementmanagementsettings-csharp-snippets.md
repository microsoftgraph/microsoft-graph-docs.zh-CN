---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0c6844d8ca377bef416d9601fd4db567c7c5b47f9df50056a3558cb55caba3a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278301"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var entitlementManagementSettings = new EntitlementManagementSettings
{
    ExternalUserLifecycleAction = "None"
};

await graphClient.IdentityGovernance.EntitlementManagement.Settings
    .Request()
    .UpdateAsync(entitlementManagementSettings);

```