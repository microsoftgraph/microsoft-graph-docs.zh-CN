---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d88ceb12a5c83de6a177fdbfca63896ef218851
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970716"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IWorkforceIntegrationCollectionPage workforceIntegrations = graphClient.teamwork().workforceIntegrations()
    .buildRequest()
    .get();

```