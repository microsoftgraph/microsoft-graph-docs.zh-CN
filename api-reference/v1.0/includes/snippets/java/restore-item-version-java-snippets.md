---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9ac14dd5b069124a6e74f4c45c6274e4e7b4eb83
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881587"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.drives("{drive-id}").items("{item-id}").versions("{version-id}")
    .restoreVersion()
    .buildRequest()
    .post();

```