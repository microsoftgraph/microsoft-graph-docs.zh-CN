---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8d5dcce916f662180af6bc8863142f99b55c3af2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881684"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = new DriveItem();
ItemReference parentReference = new ItemReference();
parentReference.id = "{new-parent-folder-id}";
driveItem.parentReference = parentReference;
driveItem.name = "new-item-name.txt";

graphClient.me().drive().items("{item-id}")
    .buildRequest()
    .patch(driveItem);

```