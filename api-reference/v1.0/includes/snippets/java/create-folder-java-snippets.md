---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4acdf548c7a4b289457712c4310abef4c82e96df
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881670"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = new DriveItem();
driveItem.name = "New Folder";
Folder folder = new Folder();
driveItem.folder = folder;
driveItem.@microsoft.graph.conflictBehavior = "rename";

graphClient.me().drive().root().children()
    .buildRequest()
    .post(driveItem);

```