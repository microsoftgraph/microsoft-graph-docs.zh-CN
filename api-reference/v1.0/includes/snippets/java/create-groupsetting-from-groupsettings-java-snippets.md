---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cead70895c467c0e8898e54e7e115f668288f354
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978287"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupSetting groupSetting = new GroupSetting();
groupSetting.displayName = "displayName-value";
groupSetting.templateId = "templateId-value";
LinkedList<SettingValue> valuesList = new LinkedList<SettingValue>();
SettingValue values = new SettingValue();
values.name = "name-value";
values.value = "value-value";
valuesList.add(values);
groupSetting.values = valuesList;

graphClient.groupSettings()
    .buildRequest()
    .post(groupSetting);

```