---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 12af199f658c466e1ad8429b35c21929150a7eac
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871943"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessParticipantActivityMinuteCountsCollectionPage getSkypeForBusinessParticipantActivityMinuteCounts = graphClient.reports()
    .getSkypeForBusinessParticipantActivityMinuteCounts('D7')
    .buildRequest()
    .get();

```