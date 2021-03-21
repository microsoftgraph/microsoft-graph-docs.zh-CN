---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af8f85aabbba5dde8b0a93f4ee4f0a1d6d95e43d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977084"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ScreenSharingRole role = ScreenSharingRole.VIEWER;

graphClient.communications().calls("{id}")
    .changeScreenSharingRole(CallChangeScreenSharingRoleParameterSet
        .newBuilder()
        .withRole(role)
        .build())
    .buildRequest()
    .post();

```