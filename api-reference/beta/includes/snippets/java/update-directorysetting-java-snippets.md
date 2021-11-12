---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8571892ed35a7267d5c963e8b72907ec9f99110d796d1974b26fb5177f5bdf74
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903820"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectorySetting directorySetting = new DirectorySetting();
LinkedList<SettingValue> valuesList = new LinkedList<SettingValue>();
SettingValue values = new SettingValue();
values.name = "name-value";
values.value = "value-value";
valuesList.add(values);
directorySetting.values = valuesList;

graphClient.settings("{id}")
    .buildRequest()
    .patch(directorySetting);

```