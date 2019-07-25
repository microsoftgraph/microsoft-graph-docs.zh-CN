---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f6d60b96387012e4aff2111361fb0ce8adfc1082
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861592"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = graphClient.me().drive().special("{name}")
    .buildRequest()
    .get();

```