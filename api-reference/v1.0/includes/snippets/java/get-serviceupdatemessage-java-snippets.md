---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5bca1f46a2eefb7e9ff791d6a0d842ca65860d5d
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58257995"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServiceUpdateMessage serviceUpdateMessage = graphClient.admin().serviceAnnouncement().messages("MC172851")
    .buildRequest()
    .get();

```