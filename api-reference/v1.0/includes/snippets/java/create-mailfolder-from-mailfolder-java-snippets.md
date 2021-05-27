---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2f57c332b323e59068e357bd382502d9405f54a
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52668789"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolder mailFolder = new MailFolder();
mailFolder.displayName = "displayName-value";
mailFolder.isHidden = true;

graphClient.me().mailFolders("{id}").childFolders()
    .buildRequest()
    .post(mailFolder);

```