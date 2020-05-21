---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c9d9d7b94a791b931abe16654499ee935407e340
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336542"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAppRoleAssignmentCollectionPage appRoleAssignments = graphClient.groups("{id}").appRoleAssignments()
    .buildRequest()
    .get();

```