---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ebc35521c7c3b58fc3a3a71066158d7d5a92a2915f591efe8fdbbe6d37b19f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220868"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().authentication().phoneMethods("3179e48a-750b-4051-897c-87b9720928f7")
    .disableSmsSignIn()
    .buildRequest()
    .post();

```