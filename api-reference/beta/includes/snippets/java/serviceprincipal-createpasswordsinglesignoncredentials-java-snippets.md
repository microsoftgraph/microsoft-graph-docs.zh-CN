---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 59403cdec2bc152c0d9ec5a9d15f93f57cece84a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970835"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String id = "5793aa3b-cca9-4794-679a240f8b58";

LinkedList<Credential> credentialsList = new LinkedList<Credential>();
Credential credentials = new Credential();
credentials.fieldId = "param_username";
credentials.value = "myusername";
credentials.type = "username";

credentialsList.add(credentials);
Credential credentials1 = new Credential();
credentials1.fieldId = "param_password";
credentials1.value = "pa$$w0rd";
credentials1.type = "password";

credentialsList.add(credentials1);

graphClient.servicePrincipals("{id}")
    .createPasswordSingleSignOnCredentials(id,credentialsList)
    .buildRequest()
    .post();

```