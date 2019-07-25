---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7f0dfd8b8d3b0996d01bc7ea5a6eade8a6de0db2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868586"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Int32 index = new Int32();

LinkedList<Json> valuesList = new LinkedList<Json>();
Json values = new Json();

valuesList.add(values);

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns()
    .add(index,values,name)
    .buildRequest()
    .post();

```