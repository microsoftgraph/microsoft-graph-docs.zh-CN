---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a230f28e722f4f3cbe4778d744cdfe530a8b04d5274c8fadae56e5496e8303f8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278877"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.roleManagement().directory().roleEligibilityScheduleRequests("{unifiedRoleEligibilityScheduleRequestsId}")
    .cancel()
    .buildRequest()
    .post();

```