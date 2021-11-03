---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1de34f903eec662f05f18712692008246978f8f6
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694559"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DeviceCollectionPage devices = graphClient.devices()
    .buildRequest()
    .select("id,extensionAttributes")
    .get();

```