---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac8f66086901e1a02145c19b1a63d1b673ff4d44fa601d378d2d31b23d2b5ed5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220270"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.communications().calls("{id}").participants("{id}")
    .buildRequest()
    .delete();

```