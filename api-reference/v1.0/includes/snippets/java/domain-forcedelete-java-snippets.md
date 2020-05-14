---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57a7d76afaf57fbdc1281eafbcbc9ea8a5c9d0ca
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "43511051"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean disableUserAccounts = true;

graphClient.domains("{id}")
    .forceDelete(disableUserAccounts)
    .buildRequest()
    .post();

```