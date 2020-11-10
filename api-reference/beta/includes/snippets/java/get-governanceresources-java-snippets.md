---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08d69c912a8222f201003e57d338038e061817db
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954389"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IGovernanceResourceCollectionPage resources = graphClient.privilegedAccess("azureResources").resources()
    .buildRequest()
    .get();

```