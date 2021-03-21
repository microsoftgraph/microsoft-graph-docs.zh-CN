---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78501f234e57ad187ad87a7c54060112508f25a2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969442"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = new DriveItem();
ItemReference parentReference = new ItemReference();
parentReference.id = "{new-parent-folder-id}";
driveItem.parentReference = parentReference;
driveItem.name = "new-item-name.txt";

graphClient.me().drive().items("{item-id}")
    .buildRequest()
    .patch(driveItem);

```