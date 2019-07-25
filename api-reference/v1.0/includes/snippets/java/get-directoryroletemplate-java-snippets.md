---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b0ab28101fa3b948826df4e37c9540038f8ad516
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888621"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryRoleTemplate directoryRoleTemplate = graphClient.directoryRoleTemplates("{id}")
    .buildRequest()
    .get();

```