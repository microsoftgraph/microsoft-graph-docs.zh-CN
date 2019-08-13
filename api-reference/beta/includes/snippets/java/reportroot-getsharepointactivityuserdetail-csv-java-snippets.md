---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cdae176cfcc204d2e7390b6a36b9603961972877
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359897"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISharePointActivityUserDetailCollectionPage getSharePointActivityUserDetail = graphClient.reports()
    .getSharePointActivityUserDetail("D7")
    .buildRequest()
    .get();

```