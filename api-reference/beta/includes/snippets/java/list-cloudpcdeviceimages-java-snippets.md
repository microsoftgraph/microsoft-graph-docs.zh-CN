---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70273ff754a88841743855af79b0b23a27f5078d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967779"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcDeviceImageCollectionPage deviceImages = graphClient.deviceManagement().virtualEndpoint().deviceImages()
    .buildRequest()
    .get();

```