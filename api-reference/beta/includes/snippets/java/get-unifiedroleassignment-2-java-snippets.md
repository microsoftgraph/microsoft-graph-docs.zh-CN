---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 846c08f62a82e4b8ce704e1c99cc4ce45a08364b
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51211077"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignment unifiedRoleAssignment = graphClient.roleManagement().directory().roleAssignments("lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1")
    .buildRequest()
    .expand("directoryScope")
    .get();

```