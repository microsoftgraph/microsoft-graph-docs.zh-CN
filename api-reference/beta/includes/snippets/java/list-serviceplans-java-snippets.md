---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a157091d819441f121ebedb8ebee6468115711f
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696243"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcServicePlanCollectionPage servicePlans = graphClient.deviceManagement().virtualEndpoint().servicePlans()
    .buildRequest()
    .get();

```