---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ad4e6e07a08053bc355807d6d509df6766b72078
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861985"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean disableUserAccounts = True;

graphClient.domains("contoso.com")
    .forceDelete(disableUserAccounts)
    .buildRequest()
    .post();

```