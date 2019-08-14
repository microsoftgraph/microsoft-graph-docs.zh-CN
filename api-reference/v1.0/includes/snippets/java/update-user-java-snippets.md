---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: adbe65253762f4563a43860e73794023cb9861cb
ms.sourcegitcommit: 3db93e28e215c0e09a65b4705ba956c6ac3b5426
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/14/2019
ms.locfileid: "36396819"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = new User();
LinkedList<String> businessPhonesList = new LinkedList<String>();
businessPhonesList.add("businessPhones-value");
user.businessPhones = businessPhonesList;
user.officeLocation = "city-value";

graphClient.me()
    .buildRequest()
    .patch(user);

```