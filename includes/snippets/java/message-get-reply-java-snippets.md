---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: abc48e058f1678971f374599a9fef5ef156ebb2e
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774643"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = graphClient.me().messages("AAMkADI4oeRpAABf0HJUAAA=")
    .buildRequest()
    .get();

```