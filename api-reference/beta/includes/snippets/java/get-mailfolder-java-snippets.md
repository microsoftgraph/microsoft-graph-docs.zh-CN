---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 388c227677318bc6d5550d6b446dd67f6cda93edf31725135ac8509f05cf2422
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279059"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolder mailFolder = graphClient.me().mailFolders("AAMkAGVmMDEzM")
    .buildRequest()
    .get();

```