---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 267409cdca95e0c8cf7bb6043b02845ba1d8b6bc
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514682"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupSetting groupSetting = new GroupSetting();
groupSetting.displayName = "Group.Unified";
groupSetting.templateId = "62375ab9-6b52-47ed-826b-58e47e0e304b";
LinkedList<SettingValue> valuesList = new LinkedList<SettingValue>();
SettingValue values = new SettingValue();
values.name = "GuestUsageGuidelinesUrl";
values.value = "https://privacy.contoso.com/privacystatement";
valuesList.add(values);
SettingValue values1 = new SettingValue();
values1.name = "EnableMSStandardBlockedWords";
values1.value = "true";
valuesList.add(values1);
SettingValue values2 = new SettingValue();
values2.name = "EnableMIPLabels";
values2.value = "true";
valuesList.add(values2);
SettingValue values3 = new SettingValue();
values3.name = "PrefixSuffixNamingRequirement";
values3.value = "[Contoso-][GroupName]";
valuesList.add(values3);
groupSetting.values = valuesList;

graphClient.groupSettings()
    .buildRequest()
    .post(groupSetting);

```