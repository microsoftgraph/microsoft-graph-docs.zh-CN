---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08eae6c3dd81fe993691f0ad6eaa4b9bc6c5ecd9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982258"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = new DriveItem();
driveItem.name = "new-file-name.docx";

graphClient.me().drive().items("{item-id}")
    .buildRequest()
    .patch(driveItem);

```