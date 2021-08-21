---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 450ede23e8c52d81ed242beefbdc15fe1bf1c14abb2a7f369f6e1b4b3ec9dfea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328752"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleAssignmentCollectionPage privilegedRoleAssignments = graphClient.privilegedRoleAssignments()
    .buildRequest()
    .filter("isElevated eq true and expirationDateTime ne null or isElevated eq false")
    .get();

```