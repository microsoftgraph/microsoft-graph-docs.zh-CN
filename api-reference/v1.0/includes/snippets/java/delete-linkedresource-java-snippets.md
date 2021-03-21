---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ffb8a2d5fb76bf6a82e0e23a905511a08a290128
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980261"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().todo().lists("dfsdc-f9dfdfs-dcsda9").tasks("e2dc-f9cce2-dce29").linkedResources("f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9")
    .buildRequest()
    .delete();

```