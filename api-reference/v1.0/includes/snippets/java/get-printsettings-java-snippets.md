---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7cd3d4d9d8df062f9763f0da3e61e442d96bd37b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777241"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintSettings printSettings = graphClient.customRequest("/print/settings", PrintSettings.class)
    .buildRequest()
    .get();

```