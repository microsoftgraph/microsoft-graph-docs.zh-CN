---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 08d69c912a8222f201003e57d338038e061817db
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859149"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IGovernanceResourceCollectionPage resources = graphClient.privilegedAccess("azureResources").resources()
    .buildRequest()
    .get();

```