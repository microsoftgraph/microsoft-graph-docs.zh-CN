---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 533473141982cf0ed5eb2a8695f7fff56f1a4a0b128cf2ed98dfee35b5f4f36f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220570"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFindRoomListsCollectionPage findRoomLists = graphClient.me()
    .findRoomLists()
    .buildRequest()
    .get();

```