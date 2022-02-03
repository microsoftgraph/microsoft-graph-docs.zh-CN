---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23c62d8fa929f57a41363d82d1cf021f428affec
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348301"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkDeviceOperation teamworkDeviceOperation = graphClient.teamwork().devices("0f3ce432-e432-0f3c-32e4-3c0f32e43c0f").operations("eab261f8-61f8-eab2-f861-b2eaf861b2ea")
    .buildRequest()
    .get();

```