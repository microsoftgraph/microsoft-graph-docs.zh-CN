---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83fef976a823114422291a5bfec33c30f31ee773
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983267"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupSetting groupSetting = new GroupSetting();
groupSetting.displayName = "GroupSettings";
groupSetting.templateId = "08d542b9-071f-4e16-94b0-74abb372e3d9";
LinkedList<SettingValue> valuesList = new LinkedList<SettingValue>();
SettingValue values = new SettingValue();
values.name = "AllowToAddGuests";
values.value = "false";
valuesList.add(values);
groupSetting.values = valuesList;

graphClient.groups("{id}").settings("{id}")
    .buildRequest()
    .patch(groupSetting);

```