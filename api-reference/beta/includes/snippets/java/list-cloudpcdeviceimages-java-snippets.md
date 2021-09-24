---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3ba9adbfaead0783dd961b3e1903930629ac15f40506cc3eb219ad6c1993a7c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105102"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcDeviceImageCollectionPage deviceImages = graphClient.deviceManagement().virtualEndpoint().deviceImages()
    .buildRequest()
    .get();

```