---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e6413904c90b397ea88614fc195eddd105f4c0c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343821"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkDeviceConfiguration teamworkDeviceConfiguration = graphClient.teamwork().devices("e19229ed-29ed-e192-ed29-92e1ed2992e1").configuration()
    .buildRequest()
    .get();

```