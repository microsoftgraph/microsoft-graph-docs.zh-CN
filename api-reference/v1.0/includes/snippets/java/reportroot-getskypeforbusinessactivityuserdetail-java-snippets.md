---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fb32324bc13bfa23eab99ed5ce4e8e6083ca116c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892488"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessActivityUserDetail('D7')
    .buildRequest()
    .get();

```