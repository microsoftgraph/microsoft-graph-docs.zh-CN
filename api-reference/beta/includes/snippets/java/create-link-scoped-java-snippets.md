---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1cdc0551444f397a85d3df9624280aae38ddd447
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137748"
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
        .withRecipients(null)
        .withRetainInheritedPermissions(null)
        .build())
    .buildRequest()
    .post();

```