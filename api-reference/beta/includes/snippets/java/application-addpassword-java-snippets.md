---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 852d5976867bcbddc777713b649d79da18c4d7bc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973554"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PasswordCredential passwordCredential = new PasswordCredential();
passwordCredential.displayName = "Password friendly name";

graphClient.applications("{id}")
    .addPassword(ApplicationAddPasswordParameterSet
        .newBuilder()
        .withPasswordCredential(passwordCredential)
        .build())
    .buildRequest()
    .post();

```