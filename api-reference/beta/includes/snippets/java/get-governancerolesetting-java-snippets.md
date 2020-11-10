---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2efd22c8f11bf00157bc160bc9842603d874c84
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965424"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GovernanceRoleSetting governanceRoleSetting = graphClient.privilegedAccess("azureResources").roleSettings("80dc5d6f-8d89-47b3-953f-01dc909ed3f9")
    .buildRequest()
    .get();

```