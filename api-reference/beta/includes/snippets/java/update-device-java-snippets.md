---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ad05c70329145bf173d23865a478e4aa204f112
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719267"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Device device = new Device();
device.accountEnabled = false;

graphClient.devices("7c06cd31-7c30-4f3b-a5c3-444cd8dd63ac")
    .buildRequest()
    .patch(device);

```