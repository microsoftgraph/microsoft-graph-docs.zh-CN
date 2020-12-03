---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dfdc458c1d87a4e829f5807c37384000e825fae0
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524381"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().permissionGrantPolicies("my-custom-consent-policy").excludes("6a846635-3e70-4a10-821e-512a0db93cbd")
    .buildRequest()
    .delete();

```