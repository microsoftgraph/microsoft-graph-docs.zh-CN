---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cd0b67397b26de1dd4cf1b20eda86c763461ddfd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878033"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean securityEnabledOnly = True;

graphClient.contacts("{id}")
    .getMemberGroups(securityEnabledOnly)
    .buildRequest()
    .post();

```