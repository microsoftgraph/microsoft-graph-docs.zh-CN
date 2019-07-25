---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 87903e4be5c2fda2cbc08df495717eaffc471f79
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893809"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getOffice365GroupsActivityStorage('D7')
    .buildRequest()
    .get();

```