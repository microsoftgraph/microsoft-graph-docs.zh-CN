---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14efdb7eaa2ee7848a0b52d26af351a6635cf524
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957309"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().authentication().phoneMethods("3179e48a-750b-4051-897c-87b9720928f7")
    .enableSmsSignIn()
    .buildRequest()
    .post();

```