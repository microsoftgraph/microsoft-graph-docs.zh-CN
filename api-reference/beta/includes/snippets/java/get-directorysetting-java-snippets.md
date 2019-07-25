---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 691b2b248297e999fa95a0bf60039241c2982a82
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862090"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectorySetting directorySetting = graphClient.settings("{id}")
    .buildRequest()
    .get();

```