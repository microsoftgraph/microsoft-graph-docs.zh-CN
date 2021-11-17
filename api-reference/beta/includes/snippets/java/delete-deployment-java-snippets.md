---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fcad134626004b043d2a8c2bfe100ecf4fce4684e5baa0c9c8570bc82d5c69e7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162672"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.admin().windows().updates().deployments("{deploymentId}")
    .buildRequest()
    .delete();

```