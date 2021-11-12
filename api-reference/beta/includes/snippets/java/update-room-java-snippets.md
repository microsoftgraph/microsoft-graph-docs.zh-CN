---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 325c93add29c845445172b8c93880ce40c09eb70f17c16b713d683c71be6c19f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163225"
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