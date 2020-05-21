---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0553579938dee551c83645755a97282aa9047da0
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335139"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUsedInsightCollectionPage used = graphClient.me().insights().used()
    .buildRequest()
    .get();

```