---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d0cf4760a5a933a9b2be8f428c0291c66fdbb88
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544205"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailSearchFolder mailFolder = new MailSearchFolder();
mailFolder.filterQuery = "contains(subject, 'Analytics')";

graphClient.me().mailFolders("AAMkAGVmMDEzM")
    .buildRequest()
    .patch(mailFolder);

```