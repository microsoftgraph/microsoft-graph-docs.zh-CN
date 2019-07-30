---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6dfdf4a6b5bbf1b866147f9f4610cdd19b6e9d00
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932683"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = new DriveItem();
driveItem.name = "Just some files";
driveItem.@name.conflictBehavior = "rename";
Bundle bundle = new Bundle();
driveItem.bundle = bundle;
LinkedList<DriveItem> childrenList = new LinkedList<DriveItem>();
DriveItem children = new DriveItem();
children.id = "1234asdf";
childrenList.add(children);
DriveItem children1 = new DriveItem();
children1.id = "1234qwerty";
childrenList.add(children1);
driveItem.children = childrenList;

graphClient.drive().bundles()
    .buildRequest()
    .post(driveItem);

```