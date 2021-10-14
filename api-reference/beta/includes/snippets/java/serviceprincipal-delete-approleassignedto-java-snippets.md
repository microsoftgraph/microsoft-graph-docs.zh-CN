---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e870637fd963e8431c05a2320f1b82b709ff583c127c21c6dd22085dd789ac4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333718"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{resource-SP-id}").appRoleAssignedTo("{appRoleAssignment-id}")
    .buildRequest()
    .delete();

```