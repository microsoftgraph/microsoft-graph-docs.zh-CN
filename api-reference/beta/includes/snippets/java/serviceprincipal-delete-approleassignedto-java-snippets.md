---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 360f6aef40d6cd00a8c3a6968709e86003dbf778
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52870190"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{resource-SP-id}").appRoleAssignedTo("{principal-id}")
    .buildRequest()
    .delete();

```