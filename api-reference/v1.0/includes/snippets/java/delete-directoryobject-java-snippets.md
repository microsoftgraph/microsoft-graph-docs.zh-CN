---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 520a38d6f200dc4d334abd92f9e62a77877f0a16
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882720"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directoryObjects("{id}")
    .buildRequest()
    .delete();

```