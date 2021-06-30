---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47994e971408392544ab158b0c08df65f7d20215
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208853"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServiceUpdateMessageCollectionPage messages = graphClient.admin().serviceAnnouncement().messages()
    .buildRequest()
    .get();

```