---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a1317a247eacbbd61ddcfc0fc64e701b2a262ed
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972682"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserPurpose userPurpose = graphClient.customRequest("/me/mailboxSettings/userPurpose", UserPurpose.class)
    .buildRequest()
    .get();

```