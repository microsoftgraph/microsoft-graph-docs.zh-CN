---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e11d57117e20f8d8435f6eac27cbd34a4e7a68b
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208381"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcUserSettingCollectionPage userSettings = graphClient.deviceManagement().virtualEndpoint().userSettings()
    .buildRequest()
    .get();

```