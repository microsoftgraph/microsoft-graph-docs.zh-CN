---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ee1bd031bbc75b1d1ce82a943acd03d64a9f2ed
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475338"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleEligibilitySchedule unifiedRoleEligibilitySchedule = graphClient.roleManagement().directory().roleEligibilitySchedules("5cfd7709-7709-5cfd-0977-fd5c0977fd5c")
    .buildRequest()
    .get();

```