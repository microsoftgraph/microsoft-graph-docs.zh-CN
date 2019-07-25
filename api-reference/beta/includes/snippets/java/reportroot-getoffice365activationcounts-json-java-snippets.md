---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f427801c7279f7ee28fa77bc4581248c334765b2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873609"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOffice365ActivationCountsCollectionPage getOffice365ActivationCounts = graphClient.reports()
    .getOffice365ActivationCounts()
    .buildRequest()
    .get();

```