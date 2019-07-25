---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 08f8dcd2e72eec5a16e99a298eb8583e5a640dd1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862028"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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