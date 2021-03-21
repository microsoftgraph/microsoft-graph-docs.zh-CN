---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: afb26494911d628564a8a214d2273eec0078adc9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982604"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkPositionCollectionPage positions = graphClient.me().profile().positions()
    .buildRequest()
    .get();

```