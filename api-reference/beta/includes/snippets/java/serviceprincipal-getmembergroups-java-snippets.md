---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4a8bd1b418ba11db5c764c2250bbc641d3af72f0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870134"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean securityEnabledOnly = True;

graphClient.servicePrincipals("{id}")
    .getMemberGroups(securityEnabledOnly)
    .buildRequest()
    .post();

```