---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 48e6578601b17cf5abe6f5263a10eff33eda6fd1
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475060"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleManagementPolicy unifiedRoleManagementPolicy = graphClient.policies().roleManagementPolicies("f93a5c37-5c37-f93a-375c-3af9375c3af9")
    .buildRequest()
    .get();

```