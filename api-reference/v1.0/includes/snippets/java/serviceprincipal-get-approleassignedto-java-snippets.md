---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f4fa45570dfe20e829e35a4ce15214f4a6b269c
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336233"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAppRoleAssignmentCollectionPage appRoleAssignedTo = graphClient.servicePrincipals("{id}").appRoleAssignedTo()
    .buildRequest()
    .get();

```