---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9fa28874d413fa1eb6c12cea6cc2e4daa009b060
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884915"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().root().workbook().worksheets("{id}")
    .range()
    .rowsBelow(count)
    .buildRequest()
    .post();

```