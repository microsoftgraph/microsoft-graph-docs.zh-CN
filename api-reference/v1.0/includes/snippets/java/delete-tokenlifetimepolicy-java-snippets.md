---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e84da1013766484f0a1568a9620e94790ec3421f
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719265"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().tokenLifetimePolicies("{id}")
    .buildRequest()
    .delete();

```