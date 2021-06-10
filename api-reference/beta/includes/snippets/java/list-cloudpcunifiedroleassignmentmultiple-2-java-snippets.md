---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef56374d0d8744dd68db98f94eff5dd90533156d
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869014"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentMultipleCollectionPage roleAssignments = graphClient.roleManagement().cloudPC().roleAssignments()
    .buildRequest()
    .filter("roleDefinitionId eq 'b5c08161-a7af-481c-ace2-a20a69a48fb1'")
    .get();

```