---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fce9ebaf91b8174bd115b5ed1d88a946814c29c1c45bf6f6a354ded22738090f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106878"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleAssignment privilegedRoleAssignment = graphClient.privilegedRoleAssignments("{id}")
    .buildRequest()
    .get();

```