---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b4a566404ca99cec3b6f5c67de994741079c353a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862790"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Device device = graphClient.devices("{id}")
    .buildRequest()
    .get();

```