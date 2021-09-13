---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72c34d7b0f13c34a21d2bbc4eb502a8e2fd1a51d439d48265d04735bf66cb8fd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278718"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String verifiedPublisherId = "1234567";

graphClient.applications("{id}")
    .setVerifiedPublisher(ApplicationSetVerifiedPublisherParameterSet
        .newBuilder()
        .withVerifiedPublisherId(verifiedPublisherId)
        .build())
    .buildRequest()
    .post();

```