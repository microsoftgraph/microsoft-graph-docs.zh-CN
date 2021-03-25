---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 360f6aef40d6cd00a8c3a6968709e86003dbf778
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208110"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{resource-SP-id}").appRoleAssignedTo("{principal-id}")
    .buildRequest()
    .delete();

```