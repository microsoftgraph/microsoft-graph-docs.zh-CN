---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6463d06eb6a4a4a7ffe790cd2471b685c8a353d3
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402695"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean securityEnabledOnly = true;

graphClient.directoryObjects("{object-id}")
    .getMemberGroups(securityEnabledOnly)
    .buildRequest()
    .post();

```