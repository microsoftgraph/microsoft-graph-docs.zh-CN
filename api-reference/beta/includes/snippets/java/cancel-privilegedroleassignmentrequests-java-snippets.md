---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c84686c40174af2813a758b7913f4e6176caf745
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977194"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.privilegedRoleAssignmentRequests("7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee")
    .cancel()
    .buildRequest()
    .post();

```