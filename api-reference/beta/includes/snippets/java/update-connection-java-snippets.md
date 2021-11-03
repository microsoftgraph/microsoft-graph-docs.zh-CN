---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e85276c56d4df4fb59f360f78911c6492f5beb5
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60689108"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalConnection externalConnection = new ExternalConnection();
externalConnection.name = "Contoso HR Service Tickets";
externalConnection.description = "Connection to index HR service tickets";

graphClient.external().connections("contosohr")
    .buildRequest()
    .patch(externalConnection);

```