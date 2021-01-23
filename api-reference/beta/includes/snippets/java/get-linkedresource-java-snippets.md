---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0f906daa56efa6ffc06b87bf10543496b52fc3a
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946161"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedResource linkedResource = graphClient.me().todo().lists("dfsdc-f9dfdfs-dcsda9").tasks("e2dc-f9cce2-dce29").linkedResources("f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9")
    .buildRequest()
    .get();

```