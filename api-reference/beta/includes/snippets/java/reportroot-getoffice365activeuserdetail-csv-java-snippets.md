---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 82f940505521940e0cb0588df19bf22d9107ed57
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360501"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOffice365ActiveUserDetailCollectionPage getOffice365ActiveUserDetail = graphClient.reports()
    .getOffice365ActiveUserDetail("D7")
    .buildRequest()
    .get();

```