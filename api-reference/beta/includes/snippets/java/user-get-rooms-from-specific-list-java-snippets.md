---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a65078cd38656fee3d2f83c241029441bd07b0d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971846"
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