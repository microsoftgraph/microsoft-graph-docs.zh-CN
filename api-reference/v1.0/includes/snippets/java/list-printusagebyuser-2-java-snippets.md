---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53868a88b42b5653c362f6b0f0ab108fd6db6bd2
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210198"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByUserCollectionPage monthlyPrintUsageByUser = graphClient.reports().monthlyPrintUsageByUser()
    .buildRequest()
    .get();

```