---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d5fe9208ba4148b2beef9a98f19903001e290a65d5512a02dde5026b9ff74c7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277392"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFindRoomsCollectionPage findRooms = graphClient.me()
    .findRooms()
    .buildRequest()
    .get();

```