---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aac21de43b31e686f9ebcceb18a86156c3cb0ea5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137750"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String type = "embed";

graphClient.me().drive().items("{item-id}")
    .createLink(DriveItemCreateLinkParameterSet
        .newBuilder()
        .withType(type)
        .withScope(null)
        .withExpirationDateTime(null)
        .withPassword(null)
        .withMessage(null)
        .withRecipients(null)
        .withRetainInheritedPermissions(null)
        .build())
    .buildRequest()
    .post();

```