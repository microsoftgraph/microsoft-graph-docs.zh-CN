---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 388f14ab372a0c5dc67b281576faa9b8c9cec9cb
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444629"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WindowsHelloForBusinessAuthenticationMethod windowsHelloForBusinessAuthenticationMethod = graphClient.users("annie@contoso.com").authentication().windowsHelloForBusinessMethods("_jpuR-TGZtk6aQCLF3BQjA2")
    .buildRequest()
    .get();

```