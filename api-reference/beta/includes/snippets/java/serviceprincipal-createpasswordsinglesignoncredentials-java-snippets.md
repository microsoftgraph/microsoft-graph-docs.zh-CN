---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e7b0bbd30a426585ce1f910a791273e53bc6bf2e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977763"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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
    .createPasswordSingleSignOnCredentials(ServicePrincipalCreatePasswordSingleSignOnCredentialsParameterSet
        .newBuilder()
        .withId(id)
        .withCredentials(credentialsList)
        .build())
    .buildRequest()
    .post();

```