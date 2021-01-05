---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8490e3baf3a05f5b7f2917de06d1fb4ffa56705d
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49754190"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean isSyncedFromOnPremises = false;

graphClient.directoryObjects()
    .getAvailableExtensionProperties(isSyncedFromOnPremises)
    .buildRequest()
    .post();

```