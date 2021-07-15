---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03ff58aeaed95a219d6c6c8091a1062226185408
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439478"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.deviceManagement().virtualEndpoint().deviceImages("{cloudPcDeviceImageId}")
    .reupload()
    .buildRequest()
    .post();

```