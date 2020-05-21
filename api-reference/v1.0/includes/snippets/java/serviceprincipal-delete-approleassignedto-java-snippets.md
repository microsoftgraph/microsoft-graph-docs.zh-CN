---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 861fdc1ab18fff14eb5a9a2e80f4fc2efb6225d5
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334274"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{id}").appRoleAssignedTo("{id}")
    .buildRequest()
    .delete();

```