---
description: 自动生成的文件。 不修改
ms.openlocfilehash: de986d75c88f36b4cb63fb8d2795e73967b47a21
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884617"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SecureScore secureScore = graphClient.security().secureScores("{id}")
    .buildRequest()
    .get();

```