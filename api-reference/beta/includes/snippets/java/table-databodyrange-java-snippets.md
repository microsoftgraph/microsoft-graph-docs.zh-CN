---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4355504a5ea67d8fa87a7f1bf6f2f5a571d66c2a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445025"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .dataBodyRange()
    .buildRequest()
    .get();

```