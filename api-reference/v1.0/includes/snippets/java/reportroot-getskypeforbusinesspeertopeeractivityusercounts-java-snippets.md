---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1930e4e96dfecc7eec7d5d263b84c5f7bd5912af
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892230"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSkypeForBusinessPeerToPeerActivityUserCounts('D7')
    .buildRequest()
    .get();

```