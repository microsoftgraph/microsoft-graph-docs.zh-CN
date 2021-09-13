---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16881487ecbdf475e5e24501290317ff526c0d872ca8cd14813d988d0b21fde6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904284"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WindowsHelloForBusinessAuthenticationMethod windowsHelloForBusinessAuthenticationMethod = graphClient.users("annie@contoso.com").authentication().windowsHelloForBusinessMethods("_jpuR-TGZtk6aQCLF3BQjA2")
    .buildRequest()
    .get();

```