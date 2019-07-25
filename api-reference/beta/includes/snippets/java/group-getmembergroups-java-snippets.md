---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a3404f328769b778295cbc9955ed7168a0975915
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858582"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean securityEnabledOnly = False;

graphClient.groups("{id}")
    .getMemberGroups(securityEnabledOnly)
    .buildRequest()
    .post();

```