---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 81bee82f40917b6213176ee3c4599592b302c893
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891079"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryRoleTemplateCollectionPage directoryRoleTemplates = graphClient.directoryRoleTemplates()
    .buildRequest()
    .get();

```