---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b08ee086176715391a62a409b619620d8ad7838af3796139b5514c70bd78dbbd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277513"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedResource linkedResource = new LinkedResource();
linkedResource.webUrl = "http://microsoft.com";
linkedResource.applicationName = "Microsoft";
linkedResource.displayName = "Microsoft";

graphClient.me().todo().lists("dfsdc-f9dfdfs-dcsda9").tasks("e2dc-f9cce2-dce29").linkedResources("f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9")
    .buildRequest()
    .patch(linkedResource);

```