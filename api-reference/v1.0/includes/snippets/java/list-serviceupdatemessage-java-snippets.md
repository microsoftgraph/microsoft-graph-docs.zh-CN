---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47994e971408392544ab158b0c08df65f7d20215
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58256939"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServiceUpdateMessageCollectionPage messages = graphClient.admin().serviceAnnouncement().messages()
    .buildRequest()
    .get();

```