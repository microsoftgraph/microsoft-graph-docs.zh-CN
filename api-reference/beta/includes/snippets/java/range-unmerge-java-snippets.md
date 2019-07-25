---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c94b8fc75c691d39e2e0a43ebf2974c7d4ec06ce
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874705"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .unmerge()
    .buildRequest()
    .post();

```