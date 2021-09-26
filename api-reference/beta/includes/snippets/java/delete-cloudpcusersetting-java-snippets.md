---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a32e2b40833b524ad94cf91404a41f6aa4e54c177cbf8515de2a5f917e71e95d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106928"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.deviceManagement().virtualEndpoint().userSettings("b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff")
    .buildRequest()
    .delete();

```