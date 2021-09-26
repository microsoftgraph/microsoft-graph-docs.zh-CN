---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6330b6ab67836e0a7ce861e6e284b296ed647205705851ceb2b9ac28df8c4fc6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162279"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.deviceManagement().virtualEndpoint().deviceImages("{cloudPcDeviceImageId}")
    .reupload()
    .buildRequest()
    .post();

```