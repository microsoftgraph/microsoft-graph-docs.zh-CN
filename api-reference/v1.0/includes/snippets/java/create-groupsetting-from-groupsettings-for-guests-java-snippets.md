---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b30ff24a0f9fe79b0dd25136db9f33f97e32176f
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412689"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupSetting groupSetting = new GroupSetting();
groupSetting.templateId = "08d542b9-071f-4e16-94b0-74abb372e3d9";
LinkedList<SettingValue> valuesList = new LinkedList<SettingValue>();
SettingValue values = new SettingValue();
values.name = "AllowToAddGuests";
values.value = "false";
valuesList.add(values);
groupSetting.values = valuesList;

graphClient.groups("055a5d18-a3a9-4338-b9c5-de92559b7ebf").settings()
    .buildRequest()
    .post(groupSetting);

```