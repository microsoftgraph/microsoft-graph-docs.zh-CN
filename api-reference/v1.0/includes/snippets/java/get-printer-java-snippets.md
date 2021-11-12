---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91b2b4e3c3744a9691dd56bf5c6435243b86e5ec2e33b2b2879bd8b7cd4ed3ef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333476"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Printer printer = graphClient.print().printers("{printerId}")
    .buildRequest()
    .get();

```