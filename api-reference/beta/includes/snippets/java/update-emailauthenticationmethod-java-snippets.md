---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1503691c422e5ea69934dcd94bfe8939d441f102e234aea9a2544bc3dba82d66
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328793"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EmailAuthenticationMethod emailAuthenticationMethod = new EmailAuthenticationMethod();
emailAuthenticationMethod.emailAddress = "kim@contoso.com";

graphClient.users("kim@contoso.com").authentication().emailMethods("3ddfcfc8-9383-446f-83cc-3ab9be4be18f")
    .buildRequest()
    .put(emailAuthenticationMethod);

```