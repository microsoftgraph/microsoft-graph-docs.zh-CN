---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 600b4b3c71455ab8cc6f5bf1371f0b6f09a3fb8d
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349028"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkDeviceHealth teamworkDeviceHealth = graphClient.teamwork().devices("d8214fe3-4fe3-d821-e34f-21d8e34f21d8").health()
    .buildRequest()
    .get();

```