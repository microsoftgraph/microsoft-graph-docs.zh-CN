---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 422703e9d1fdd1c13f616fbc7431a544d032e80e
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207323"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcUserSetting cloudPcUserSetting = graphClient.deviceManagement().virtualEndpoint().userSettings("556092f8-92f8-5560-f892-6055f8926055")
    .buildRequest()
    .get();

```