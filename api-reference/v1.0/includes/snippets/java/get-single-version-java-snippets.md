---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9845497a990db23e7c7766909f7262b57ba6b639
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886465"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItemVersion driveItemVersion = graphClient.me().drive().items("{item-id}").versions("{version-id}")
    .buildRequest()
    .get();

```