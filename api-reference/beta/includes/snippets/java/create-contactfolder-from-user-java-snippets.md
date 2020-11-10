---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5fddb100a83d585df59f4b869c099af10498ee31
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968559"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContactFolder contactFolder = new ContactFolder();
contactFolder.parentFolderId = "parentFolderId-value";
contactFolder.displayName = "displayName-value";

graphClient.me().contactFolders()
    .buildRequest()
    .post(contactFolder);

```