---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f00adc50b6ffeaaeb30cb589e655281e8a46fa14a918201a2e07e01a42be9819
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409096"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = new DriveItem();
driveItem.name = "New Folder";
Folder folder = new Folder();
driveItem.folder = folder;
driveItem.additionalDataManager().put("@microsoft.graph.conflictBehavior", new JsonPrimitive("rename"));

graphClient.me().drive().root().children()
    .buildRequest()
    .post(driveItem);

```