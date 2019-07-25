---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4f2b169d63961b33cb35f09dc532498d5bd597a3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874831"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String shift = "shift-value";

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .insert(shift)
    .buildRequest()
    .post();

```