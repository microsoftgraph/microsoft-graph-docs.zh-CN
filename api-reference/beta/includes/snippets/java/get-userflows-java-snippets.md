---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34746b9940cb991545236075ab26e5cfb7293bcf
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953212"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IIdentityUserFlowCollectionPage userFlows = graphClient.identity().userFlows()
    .buildRequest()
    .get();

```