---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b358add10097b3bec1805627de0b0893fc0b291e31a531b81b57823b5702a50
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278267"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleEligibilityScheduleRequestCollectionPage roleEligibilityScheduleRequests = graphClient.roleManagement().directory().roleEligibilityScheduleRequests()
    .buildRequest()
    .get();

```