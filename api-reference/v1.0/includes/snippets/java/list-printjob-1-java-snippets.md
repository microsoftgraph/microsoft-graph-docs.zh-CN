---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a0266925bfb819746ffb6e47a2165395356888e
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210909"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintJobCollectionPage jobs = graphClient.print().printers("{printerId}").jobs()
    .buildRequest()
    .get();

```