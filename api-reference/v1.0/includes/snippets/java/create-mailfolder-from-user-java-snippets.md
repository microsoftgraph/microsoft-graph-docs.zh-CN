---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da6b84e7216b0e52e70eb760bd0b35fc78db00c7
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49661836"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolder mailFolder = new MailFolder();
mailFolder.displayName = "Clutter";

graphClient.me().mailFolders()
    .buildRequest()
    .post(mailFolder);

```