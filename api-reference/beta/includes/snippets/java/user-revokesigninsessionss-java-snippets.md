---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dbff260239ca5d7bd36e6a3ba4d5a32df95622a0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983992"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me()
    .revokeSignInSessions()
    .buildRequest()
    .post();

```