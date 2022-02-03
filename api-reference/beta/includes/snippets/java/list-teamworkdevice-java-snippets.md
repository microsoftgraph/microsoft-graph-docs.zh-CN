---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 048ed0484da4550f0eac3ea39242c8f0716b5861
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62342570"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkDeviceCollectionPage devices = graphClient.teamwork().devices()
    .buildRequest()
    .get();

```