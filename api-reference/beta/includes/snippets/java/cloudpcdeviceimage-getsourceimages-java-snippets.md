---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38b96cdd9ea7ac04a0f55deafe8f59c1b5c10631
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976526"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcDeviceImageGetSourceImagesCollectionPage getSourceImages = graphClient.deviceManagement().virtualEndpoint().deviceImages()
    .getSourceImages()
    .buildRequest()
    .get();

```