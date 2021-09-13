---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a059939a22828932a5e0a489fb04dd9abadc90186d7d3c5148141e6eb3564f2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277680"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryRole directoryRole = graphClient.directoryRoles("23f3b4b4-8a29-4420-8052-e4950273bbda")
    .buildRequest()
    .get();

```