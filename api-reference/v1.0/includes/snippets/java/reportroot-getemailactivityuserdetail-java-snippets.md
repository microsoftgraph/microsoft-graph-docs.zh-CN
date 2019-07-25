---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a869969d6e2f206175db3c6be3252d0c3b4293b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891864"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getEmailActivityUserDetail('D7')
    .buildRequest()
    .get();

```