---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6a738effbe120b4dc5602852fdfde00cc322889f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893915"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOffice365GroupsActivityGroupCounts('D7')
    .buildRequest()
    .get();

```