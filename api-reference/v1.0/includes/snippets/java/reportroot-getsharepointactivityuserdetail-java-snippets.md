---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c574dcce31f5ab87b353be287c5c5679e3c77531
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893467"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSharePointActivityUserDetail('D7')
    .buildRequest()
    .get();

```