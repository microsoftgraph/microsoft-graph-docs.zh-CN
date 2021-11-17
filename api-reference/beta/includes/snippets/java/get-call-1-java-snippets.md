---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa763aeb1456caf903aa3c738fa8c616a8dfeac4385202da605c2f5ca698463f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158323"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Call call = graphClient.communications().calls("{id}")
    .buildRequest()
    .get();

```