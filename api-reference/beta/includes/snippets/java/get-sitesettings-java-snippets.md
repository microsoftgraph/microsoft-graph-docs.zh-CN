---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 14735bbf2d2e46239742f466f0d575db793ac397
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211187"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SiteSettings siteSettings = graphClient.customRequest("/sites/03164a2b-a288-486a-993e-c41454113e2a/settings", SiteSettings.class)
    .buildRequest()
    .get();

```