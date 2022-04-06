---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f2d78ec6209c742626054057e97a735dd033051
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757691"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = new DriveItem();
driveItem.name = "My Day at the Beach";
driveItem.additionalDataManager().put("@microsoft.graph.conflictBehavior", new JsonPrimitive("rename"));
Bundle bundle = new Bundle();
Album album = new Album();
bundle.album = album;
driveItem.bundle = bundle;
LinkedList<DriveItem> childrenList = new LinkedList<DriveItem>();
DriveItem children = new DriveItem();
children.id = "1234asdf";
childrenList.add(children);
DriveItemCollectionResponse driveItemCollectionResponse = new DriveItemCollectionResponse();
driveItemCollectionResponse.value = childrenList;
DriveItemCollectionPage driveItemCollectionPage = new DriveItemCollectionPage(driveItemCollectionResponse, null);
driveItem.children = driveItemCollectionPage;

graphClient.drive().bundles()
    .buildRequest()
    .post(driveItem);

```