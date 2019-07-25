---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d615a773ac576131b80d88883de6d168b1e17b6a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855401"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Alert alert = graphClient.security().alerts("{id}")
    .buildRequest()
    .get();

```