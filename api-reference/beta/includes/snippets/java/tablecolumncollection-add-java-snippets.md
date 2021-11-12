---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00c91b69d1be2386bf461a8fe6f86a70d36e2475d3e7d4ac9062c449e2d405d2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333384"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

int index = new int();

LinkedList<JsonElement> valuesList = new LinkedList<JsonElement>();
JsonElement values = new JsonObject();

valuesList.add(values);

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns()
    .add(WorkbookTableColumnAddParameterSet
        .newBuilder()
        .withIndex(index)
        .withValues(values)
        .withName(null)
        .build())
    .buildRequest()
    .post();

```