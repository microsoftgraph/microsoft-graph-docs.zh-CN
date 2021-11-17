---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 07cb4ed3b935a2f3ed5f6a02300106288b33efffd0538453e75e02682ae8a1d1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903676"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTask outlookTask = graphClient.me().outlook().tasks("AAMkADA1MTrgAAA=")
    .buildRequest()
    .get();

```