---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8aa4b8311e22f5b59f5487c61bdd856498b6d0f6fc9b9c412f2345108b96e170
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163779"
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
    .updatePasswordSingleSignOnCredentials(ServicePrincipalUpdatePasswordSingleSignOnCredentialsParameterSet
        .newBuilder()
        .withId(id)
        .withCredentials(credentialsList)
        .build())
    .buildRequest()
    .post();

```