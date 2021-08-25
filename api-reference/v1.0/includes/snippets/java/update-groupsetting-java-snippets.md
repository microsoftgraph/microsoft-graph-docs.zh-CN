---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc9e2b51c3cb8c9b774fa81374bb44c704565764
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514623"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupSetting groupSetting = new GroupSetting();
LinkedList<SettingValue> valuesList = new LinkedList<SettingValue>();
SettingValue values = new SettingValue();
values.name = "AllowToAddGuests";
values.value = "true";
valuesList.add(values);
groupSetting.values = valuesList;

graphClient.groups("0167b5af-f3d1-4910-82d2-398747fa381c").settings("fa6df613-159b-4f94-add2-7093f961900b")
    .buildRequest()
    .patch(groupSetting);

```