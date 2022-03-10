---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2dd2910228ace13effd129a477db23b9df0d45b3
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411675"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectorySetting directorySetting = new DirectorySetting();
LinkedList<SettingValue> valuesList = new LinkedList<SettingValue>();
SettingValue values = new SettingValue();
values.name = "CustomBlockedWordsList";
values.value = "Contoso";
valuesList.add(values);
directorySetting.values = valuesList;

graphClient.settings("3c105fc3-2254-4861-9e2d-d59e2126f3ef")
    .buildRequest()
    .patch(directorySetting);

```