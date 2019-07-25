---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0e699efdd7fe7702461a76b5b796aae0f63bf45d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891593"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SignIn signIn = graphClient.auditLogs().signIns("{id}")
    .buildRequest()
    .get();

```