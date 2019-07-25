---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 351a91d3af7d2d258aa7bc9b75a84d34eb6831b4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886893"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().root().workbook().worksheets("{id}")
    .range()
    .columnsAfter(count)
    .buildRequest()
    .post();

```