---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 98b37d57e3fb605ab1b687b91bd6c7301c31f687
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35894194"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

int index = 3;

LinkedList<Json> valuesList = new LinkedList<Json>();
Json values = new Json();

valuesList.add(values);

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns()
    .add(index,values,name)
    .buildRequest()
    .post();

```