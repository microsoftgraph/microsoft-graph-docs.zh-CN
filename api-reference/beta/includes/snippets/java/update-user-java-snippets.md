---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7a8f3c39833466fc8e35b3d5a666466bb493224
ms.sourcegitcommit: d09d720b56ed6f1fad556e2a3730c2e850db355f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/02/2020
ms.locfileid: "49556177"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = new User();
LinkedList<String> businessPhonesList = new LinkedList<String>();
businessPhonesList.add("+1 425 555 0109");
user.businessPhones = businessPhonesList;
user.officeLocation = "18/2111";

graphClient.me()
    .buildRequest()
    .patch(user);

```