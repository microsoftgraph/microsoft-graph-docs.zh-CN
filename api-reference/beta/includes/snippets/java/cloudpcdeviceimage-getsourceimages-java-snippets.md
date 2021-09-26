---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a892adb66d6c1f5596b0a7b7360919796aa25f21f98bb9c933fd2277d837483b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57331987"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcDeviceImageGetSourceImagesCollectionPage getSourceImages = graphClient.deviceManagement().virtualEndpoint().deviceImages()
    .getSourceImages()
    .buildRequest()
    .get();

```