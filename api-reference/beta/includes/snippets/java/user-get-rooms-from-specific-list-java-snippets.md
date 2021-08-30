---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d45d45e80eda371d5aeca1648efa223b6ae224786d50d762bdbf8ea09fa1d6ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277393"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFindRoomsCollectionPage findRooms = graphClient.me()
    .findRooms(UserFindRoomsParameterSet
        .newBuilder()
        .withRoomList("Building2Rooms@contoso.onmicrosoft.com")
        .build())
    .buildRequest()
    .get();

```