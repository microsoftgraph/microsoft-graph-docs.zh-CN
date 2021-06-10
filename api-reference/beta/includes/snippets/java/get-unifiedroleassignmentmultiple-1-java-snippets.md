---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89d270a613dbf8350a82bda5ede3401c431ef3dd
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869987"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentMultiple unifiedRoleAssignmentMultiple = graphClient.roleManagement().cloudPC().roleAssignments("dbe9d288-fd87-41f4-b33d-b498ed207096")
    .buildRequest()
    .get();

```