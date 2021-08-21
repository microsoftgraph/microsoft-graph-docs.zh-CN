---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ee668d92594dd7223cae7cafb595cf68539cb5b567d27df7a13290e4f0ea2e8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219840"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleEligibilityScheduleInstance unifiedRoleEligibilityScheduleInstance = graphClient.roleManagement().directory().roleEligibilityScheduleInstances("5cfd7709-7709-5cfd-0977-fd5c0977fd5c")
    .buildRequest()
    .get();

```