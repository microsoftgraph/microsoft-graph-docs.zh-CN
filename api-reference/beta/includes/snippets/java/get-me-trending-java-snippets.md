---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 381820ffda5d6c302a27638f5d0ffa4ca3373e6c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50984366"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TrendingCollectionPage trending = graphClient.me().insights().trending()
    .buildRequest()
    .get();

```