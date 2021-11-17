---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4500c826879a5d2a7e3fbb682abc25d4a7a3af1e35e1255e4ca36d0dcbd9de0a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332498"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EntitlementManagementSettings entitlementManagementSettings = new EntitlementManagementSettings();
entitlementManagementSettings.externalUserLifecycleAction = "None";

graphClient.identityGovernance().entitlementManagement().settings()
    .buildRequest()
    .patch(entitlementManagementSettings);

```