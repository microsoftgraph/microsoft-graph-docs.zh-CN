---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff6976d8ff9d60dbbd9fde62cabc2951ec789e2b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971312"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String type = "edit";

String scope = "organization";

graphClient.me().drive().items("{item-id}")
    .createLink(DriveItemCreateLinkParameterSet
        .newBuilder()
        .withType(type)
        .withScope(scope)
        .withExpirationDateTime(null)
        .withPassword(null)
        .withMessage(null)
        .build())
    .buildRequest()
    .post();

```