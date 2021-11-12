---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ac044882eb273c89b58561705824c4bbab0758d58783379383a36c8280343ce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333109"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = graphClient.me().messages("AAMkAGVmMDEz")
    .buildRequest()
    .select("internetMessageHeaders")
    .get();

```