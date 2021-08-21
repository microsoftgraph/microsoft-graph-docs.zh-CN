---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3aa450b509b8537ac9fb6cc02474346ce7b6888a795995a3aa75ccba0050bec1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273949"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleAssignmentCollectionPage privilegedRoleAssignments = graphClient.privilegedRoleAssignments()
    .buildRequest()
    .get();

```