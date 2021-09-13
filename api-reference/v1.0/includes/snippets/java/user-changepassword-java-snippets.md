---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29357b304f8bf3928aa34d74b1619420ec4e3dbdc9126c9ddeba418ae1748ed4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164228"
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