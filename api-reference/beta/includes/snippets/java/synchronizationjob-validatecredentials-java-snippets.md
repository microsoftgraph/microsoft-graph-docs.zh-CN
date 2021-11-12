---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7783c5cc6b45924ebabf576f17d045007986b3ec6dc2e907c0527335655fdf24
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220194"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<SynchronizationSecretKeyStringValuePair> credentialsList = new LinkedList<SynchronizationSecretKeyStringValuePair>();
SynchronizationSecretKeyStringValuePair credentials = new SynchronizationSecretKeyStringValuePair();
credentials.key = SynchronizationSecret.USER_NAME;
credentials.value = "user@domain.com";

credentialsList.add(credentials);
SynchronizationSecretKeyStringValuePair credentials1 = new SynchronizationSecretKeyStringValuePair();
credentials1.key = SynchronizationSecret.PASSWORD;
credentials1.value = "password-value";

credentialsList.add(credentials1);

graphClient.servicePrincipals("{id}").synchronization().jobs("{id}")
    .validateCredentials(SynchronizationJobValidateCredentialsParameterSet
        .newBuilder()
        .withApplicationIdentifier(null)
        .withTemplateId(null)
        .withUseSavedCredentials(null)
        .withCredentials(credentialsList)
        .build())
    .buildRequest()
    .post();

```