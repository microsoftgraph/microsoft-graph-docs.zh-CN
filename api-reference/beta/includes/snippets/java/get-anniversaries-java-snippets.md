---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49142a43cec9eb7e0f3ab5beeaa78dda29594a22ca10e10a8758cfcd1fba181b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273856"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAnnualEventCollectionPage anniversaries = graphClient.me().profile().anniversaries()
    .buildRequest()
    .get();

```