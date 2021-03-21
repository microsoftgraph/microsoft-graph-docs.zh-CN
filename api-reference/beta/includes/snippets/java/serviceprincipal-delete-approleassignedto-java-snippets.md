---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62572b792722edff5caa6e5f358376b3944c8d8c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960733"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{id}").appRoleAssignedTo("{id}")
    .buildRequest()
    .delete();

```