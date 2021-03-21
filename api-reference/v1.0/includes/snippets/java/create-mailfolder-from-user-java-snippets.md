---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6cb125c6acb79dad9d7f3eb66ae7c7b6d22575ae
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973497"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolder mailFolder = new MailFolder();
mailFolder.displayName = "Clutter";

graphClient.me().mailFolders()
    .buildRequest()
    .post(mailFolder);

```