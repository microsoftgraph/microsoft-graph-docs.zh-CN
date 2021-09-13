---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ddded490679de564a6864e363f8d95e45ecd2504bf70f1c7eff6efe049d56e88
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378775"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalConnection externalConnection = new ExternalConnection();
externalConnection.name = "Contoso HR Service Tickets";
externalConnection.description = "Connection to index HR service tickets";

graphClient.connections("contosohr")
    .buildRequest()
    .patch(externalConnection);

```