---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4124e0b9b530729ef84adddce998c32c1e9cca1f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978050"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectorySetting directorySetting = new DirectorySetting();
directorySetting.templateId = "templateId-value";
LinkedList<SettingValue> valuesList = new LinkedList<SettingValue>();
SettingValue values = new SettingValue();
values.name = "name-value";
values.value = "value-value";
valuesList.add(values);
directorySetting.values = valuesList;

graphClient.settings()
    .buildRequest()
    .post(directorySetting);

```