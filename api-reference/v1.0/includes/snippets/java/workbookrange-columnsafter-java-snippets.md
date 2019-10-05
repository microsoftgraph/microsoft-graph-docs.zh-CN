---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c57e04eaf3067f663c4cb7a90321c297a13bfe43
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402948"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().root().workbook().worksheets("{id}")
    .range()
    .columnsAfter(null)
    .buildRequest()
    .post();

```