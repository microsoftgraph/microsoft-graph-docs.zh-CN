---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c5b5a833f6fa12bebb11761236d86425b08cce10
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887223"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = graphClient.me().messages("AAMkADYAAAImV_lAAA=")
    .buildRequest()
    .get();

```