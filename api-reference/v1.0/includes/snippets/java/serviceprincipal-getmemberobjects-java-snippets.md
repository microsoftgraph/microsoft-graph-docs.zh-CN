---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a09168a6b39767c56e40d4df54f2ab22f6897953
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336269"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean securityEnabledOnly = true;

graphClient.servicePrincipals("{id}")
    .getMemberObjects(securityEnabledOnly)
    .buildRequest()
    .post();

```