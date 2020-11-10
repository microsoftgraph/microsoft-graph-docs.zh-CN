---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82de4f0e6703e7156073318395dfe36e89530065
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980298"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISynchronizationSchemaFilterOperatorsCollectionPage filterOperators = graphClient.servicePrincipals("{id}").synchronization().jobs("{jobId}").schema()
    .filterOperators()
    .buildRequest()
    .get();

```