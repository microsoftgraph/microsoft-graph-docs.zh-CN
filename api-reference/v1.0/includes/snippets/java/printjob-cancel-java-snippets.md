---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc7d6314e4c8cf9cc61d812446a1cb71ccec90db981299485f7cf1852094b97a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162554"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().printers("{printerId}").jobs("{printJobId}")
    .cancel()
    .buildRequest()
    .post();

```