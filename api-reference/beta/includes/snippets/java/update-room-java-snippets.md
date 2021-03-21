---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 499a874791d2a4df7b21590cd3d0283b33c2d183
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980949"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Room place = new Room();
place.nickname = "Conf Room";
place.building = "1";
place.label = "100";
place.capacity = 50;
place.isWheelChairAccessible = false;

graphClient.places("cf100@contoso.com")
    .buildRequest()
    .patch(place);

```