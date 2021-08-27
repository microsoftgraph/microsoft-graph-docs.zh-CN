---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1b7e4699e3fee256c437ecdb9073d4923db7bf621199d9c9f430a30ed13c267
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333483"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().identityProviders("{id}")
    .buildRequest()
    .delete();

```