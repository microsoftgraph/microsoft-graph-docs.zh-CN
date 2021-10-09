---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6ec4f51fb5123e73f62a61209e7b2764fedfd10447b288eda3a29a581605ccb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278406"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryRole directoryRole = graphClient.directoryRoles("fe8f10bf-c9c2-47eb-95cb-c26cc85f1830")
    .buildRequest()
    .get();

```