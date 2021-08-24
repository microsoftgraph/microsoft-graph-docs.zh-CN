---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a1ac1fb1c0f2d86559949fbca379f2cdd99ad8a1fc85a4461c276ad0bc914c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220209"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SignInCollectionPage signIns = graphClient.auditLogs().signIns()
    .buildRequest()
    .get();

```