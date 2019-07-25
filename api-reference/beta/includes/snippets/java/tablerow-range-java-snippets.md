---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 87b94260c9bd9f5f7b972353879fafaebde78c8c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868516"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").rows("{index}")
    .range()
    .buildRequest()
    .post();

```