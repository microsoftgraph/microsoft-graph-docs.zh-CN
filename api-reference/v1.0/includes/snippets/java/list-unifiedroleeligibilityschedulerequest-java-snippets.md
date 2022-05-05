---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18198c7ca6fccf578e1f1a6fe2739cec88523e20
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207027"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleEligibilityScheduleRequestCollectionPage roleEligibilityScheduleRequests = graphClient.roleManagement().directory().roleEligibilityScheduleRequests()
    .buildRequest()
    .get();

```