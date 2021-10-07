---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2018e5ee2854273b2be3ea7885a15c37904ce07
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214429"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcSupportedRegionCollectionPage supportedRegions = graphClient.deviceManagement().virtualEndpoint().supportedRegions()
    .buildRequest()
    .get();

```