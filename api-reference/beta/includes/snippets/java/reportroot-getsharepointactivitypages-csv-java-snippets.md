---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 323a51d9118ef1d6efcc23462125e49feca613fd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359875"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISharePointActivityPagesCollectionPage getSharePointActivityPages = graphClient.reports()
    .getSharePointActivityPages("D7")
    .buildRequest()
    .get();

```