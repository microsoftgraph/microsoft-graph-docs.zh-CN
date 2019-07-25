---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4146912c0c36ba229f96837a131377eae4c0e56c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863120"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IContractCollectionPage contracts = graphClient.contracts()
    .buildRequest()
    .get();

```