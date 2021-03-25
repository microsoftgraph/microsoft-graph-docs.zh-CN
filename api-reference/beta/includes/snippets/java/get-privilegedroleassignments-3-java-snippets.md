---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f13edad84a6778b5c034c68f6371188695997288
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209589"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleAssignmentCollectionPage privilegedRoleAssignments = graphClient.privilegedRoleAssignments()
    .buildRequest()
    .filter("isElevated eq true and expirationDateTime eq null")
    .get();

```