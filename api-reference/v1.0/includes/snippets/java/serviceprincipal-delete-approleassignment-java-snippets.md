---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6ee0d78426fd10919abb9c6a55437094f71b3a7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974628"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{id}").appRoleAssignments("{id}")
    .buildRequest()
    .delete();

```