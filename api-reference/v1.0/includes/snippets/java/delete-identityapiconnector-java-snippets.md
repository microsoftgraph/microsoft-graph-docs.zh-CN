---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25e9a7f8f76f89914cffc25bb81940c84516337407fa08ac32ba7f0d9fbbe45a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219348"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().apiConnectors("370eeb68-dfd3-4a47-8160-8824c2358321")
    .buildRequest()
    .delete();

```