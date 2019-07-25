---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b02ac8cdcfc8ab86b996035be6ceb5ec75ba1a06
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880445"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directory().deletedItems("{object-id}")
    .restore()
    .buildRequest()
    .post();

```