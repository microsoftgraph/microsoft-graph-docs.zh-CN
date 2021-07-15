---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3786642415644ab569f61002afada94e48800dc7
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442817"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String currentPassword = "xWwvJ]6NMw+bWH-d";

String newPassword = "0eM85N54wFxWwvJ]";

graphClient.me()
    .changePassword(UserChangePasswordParameterSet
        .newBuilder()
        .withCurrentPassword(currentPassword)
        .withNewPassword(newPassword)
        .build())
    .buildRequest()
    .post();

```