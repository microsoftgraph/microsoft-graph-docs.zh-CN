---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16e3b5a0d0fa70105f908ccbaa3cfd4394af40abca34c5d43f3c170aa8faa2b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278473"
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
        .build())
    .buildRequest()
    .post();

```