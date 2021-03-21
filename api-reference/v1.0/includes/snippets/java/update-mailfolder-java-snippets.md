---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b805d45d9e8638fb0f5f939e75411475f724692
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981720"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolder mailFolder = new MailFolder();
mailFolder.displayName = "displayName-value";

graphClient.me().mailFolders("{id}")
    .buildRequest()
    .patch(mailFolder);

```