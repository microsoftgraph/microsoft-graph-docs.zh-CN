---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a710246e1a56abbb014ecaba5565a7d8bbee1533
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433784"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .totalRowRange()
    .buildRequest()
    .get();

```