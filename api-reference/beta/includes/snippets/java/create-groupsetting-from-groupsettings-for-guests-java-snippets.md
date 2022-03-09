---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7b7e57833fd0ecb7f306bc60ce5da09d7b25614
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395732"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectorySetting directorySetting = new DirectorySetting();
directorySetting.templateId = "08d542b9-071f-4e16-94b0-74abb372e3d9";
LinkedList<SettingValue> valuesList = new LinkedList<SettingValue>();
SettingValue values = new SettingValue();
values.name = "AllowToAddGuests";
values.value = "false";
valuesList.add(values);
directorySetting.values = valuesList;

graphClient.groups("05aa6a98-956a-45c0-b13b-88076a23f2cd").settings()
    .buildRequest()
    .post(directorySetting);

```