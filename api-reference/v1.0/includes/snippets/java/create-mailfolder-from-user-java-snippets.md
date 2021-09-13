---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3fc5c4aba8cea64f81ef3f36d449751375bad829cb0076d4d89d557b3c182394
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103766"
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