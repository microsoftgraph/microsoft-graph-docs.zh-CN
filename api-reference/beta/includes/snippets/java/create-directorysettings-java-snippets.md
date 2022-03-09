---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f153de481969d4f9711f470fa9f8d645bdff28c9
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395718"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectorySetting directorySetting = new DirectorySetting();
directorySetting.templateId = "62375ab9-6b52-47ed-826b-58e47e0e304b";
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
directorySetting.values = valuesList;

graphClient.settings()
    .buildRequest()
    .post(directorySetting);

```