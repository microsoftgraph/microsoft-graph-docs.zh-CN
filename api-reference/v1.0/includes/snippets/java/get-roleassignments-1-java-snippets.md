---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 847554b2e3198c5e740b4594c8e87fe0b09d3edf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59130418"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentCollectionPage roleAssignments = graphClient.roleManagement().directory().roleAssignments()
    .buildRequest()
    .filter("roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'")
    .expand("principal")
    .get();

```