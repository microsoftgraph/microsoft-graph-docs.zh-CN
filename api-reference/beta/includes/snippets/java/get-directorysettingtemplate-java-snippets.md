---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b6969d064ddb854b2289c3eae702bf5a6f5d7206
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862002"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectorySettingTemplate directorySettingTemplate = graphClient.directorySettingTemplates("{id}")
    .buildRequest()
    .get();

```