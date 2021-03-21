---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7ad4cbcd53345db1d1060f89b6f2315eafd3cd7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980287"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolder mailFolder = new MailFolder();
mailFolder.displayName = "Clutter";
mailFolder.isHidden = true;

graphClient.me().mailFolders()
    .buildRequest()
    .post(mailFolder);

```