---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9fde2bd98e90a419c02b2af4a7eb5fc312c61b5f
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334415"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PasswordCredential passwordCredential = new PasswordCredential();
passwordCredential.displayName = "Password friendly name";

graphClient.servicePrincipals("{id}")
    .addPassword(passwordCredential)
    .buildRequest()
    .post();

```