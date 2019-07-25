---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 63235871bc4532c6f1e28f8491a2da41592a5733
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892305"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessParticipantActivityMinuteCounts('D7')
    .buildRequest()
    .get();

```