---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3aa6a499f77e1d7e1270b0891f70fcb49ec3ec0d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308487"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEmailAppUsageUserDetailCollectionPage getEmailAppUsageUserDetail = graphClient.reports()
    .getEmailAppUsageUserDetail("D7")
    .buildRequest()
    .get();

```