---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f3dc5dd7720d34e443b4a62330750ed21bc7b54
ms.sourcegitcommit: df2c52f84aae5d4fed641d7411ba547371f0eaad
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2020
ms.locfileid: "44055586"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String type = "view";

String password = "ThisIsMyPrivatePassword";

String scope = "anonymous";

graphClient.me().drive().items("{item-id}")
    .createLink(type,scope,null,password,null)
    .buildRequest()
    .post();

```