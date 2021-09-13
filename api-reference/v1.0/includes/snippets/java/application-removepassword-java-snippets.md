---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13020262a37af98ddc5f988cc7f2365b28a61e9af2b7abf94a4e189374fec701
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902339"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UUID keyId = UUID.fromString("f0b0b335-1d71-4883-8f98-567911bfdca6");

graphClient.applications("{id}")
    .removePassword(ApplicationRemovePasswordParameterSet
        .newBuilder()
        .withKeyId(keyId)
        .build())
    .buildRequest()
    .post();

```