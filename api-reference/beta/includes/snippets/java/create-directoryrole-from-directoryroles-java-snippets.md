---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72a27a96d697191b989e3fa78fdc45dc4049da74
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "53005772"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryRole directoryRole = new DirectoryRole();
directoryRole.roleTemplateId = "fe930be7-5e62-47db-91af-98c3a49a38b1";

graphClient.directoryRoles()
    .buildRequest()
    .post(directoryRole);

```