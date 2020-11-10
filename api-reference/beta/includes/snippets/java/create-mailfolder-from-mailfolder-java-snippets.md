---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0cfe1b5b504f0385a00825bb5b786f732487dfe3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979223"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolder mailFolder = new MailFolder();
mailFolder.displayName = "displayName-value";

graphClient.me().mailFolders("{id}").childFolders()
    .buildRequest()
    .post(mailFolder);

```