---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab2bce3665170083d9fb22d4fe1e95ac3e2e78b9
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507222"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContactFolder contactFolder = new ContactFolder();
contactFolder.displayName = "Family";

graphClient.me().contactFolders("{id}").childFolders()
    .buildRequest()
    .post(contactFolder);

```