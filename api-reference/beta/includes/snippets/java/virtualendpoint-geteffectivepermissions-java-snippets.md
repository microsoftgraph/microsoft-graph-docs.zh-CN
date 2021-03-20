---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad6ee7365eef6fa885b6f8986d7ab20ba663dbfb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974958"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

VirtualEndpointGetEffectivePermissionsCollectionPage getEffectivePermissions = graphClient.deviceManagement().virtualEndpoint()
    .getEffectivePermissions()
    .buildRequest()
    .get();

```