---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d472707b1b7d0b229554e903d4444e2a48e65df
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870196"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServicePrincipal servicePrincipal = graphClient.servicePrincipals("{id}")
    .buildRequest()
    .get();

```