---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de22441831788013cf75bad6b33c6d47094470ce
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973598"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Printer printer = graphClient.print().printers("{printerId}")
    .buildRequest()
    .select("id,displayName,capabilities")
    .get();

```