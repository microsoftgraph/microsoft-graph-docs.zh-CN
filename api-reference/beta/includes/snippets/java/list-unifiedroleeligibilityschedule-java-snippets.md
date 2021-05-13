---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8aa95f391ac61cbaf09369c309124878b6531dd8
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475303"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleEligibilityScheduleCollectionPage roleEligibilitySchedules = graphClient.roleManagement().directory().roleEligibilitySchedules()
    .buildRequest()
    .get();

```