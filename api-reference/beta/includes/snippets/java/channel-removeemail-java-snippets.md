---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a48ea091949d8795c9512ed68821042795f68b9a19a4c1d9160fc57acdcb9f5b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902853"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("893075dd-2487-4122-925f-022c42e20265").channels("19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2")
    .removeEmail()
    .buildRequest()
    .post();

```