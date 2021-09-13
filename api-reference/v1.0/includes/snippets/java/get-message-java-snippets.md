---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3689c4cbe8daa285efab04af9eaca81a4c836eaefc23899c51973fa6338997e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218772"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = graphClient.me().messages("AAMkADhMGAAA=")
    .buildRequest()
    .get();

```