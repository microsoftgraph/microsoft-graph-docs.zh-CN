---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4fbd005300aac32ff94f9ceac1c8ead664bcd826
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881336"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = graphClient.me().messages("AAMkADhMGAAA=")
    .buildRequest()
    .get();

```