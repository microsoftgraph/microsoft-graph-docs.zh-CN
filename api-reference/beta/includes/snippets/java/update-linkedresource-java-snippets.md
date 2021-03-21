---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba0ef910c13fa8dfb231e79d76becc75a479c4a9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967146"
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