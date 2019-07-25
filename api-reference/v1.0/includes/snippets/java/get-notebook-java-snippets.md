---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3d1c8838c60338b06c9960d773d8aaabf7306e53
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890204"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Notebook notebook = graphClient.me().onenote().notebooks("{id}")
    .buildRequest()
    .get();

```