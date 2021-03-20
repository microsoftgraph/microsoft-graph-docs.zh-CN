---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c875cd9f7b1c87b1093be20d900c8b32bbfbba4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976292"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Calendar calendar = graphClient.me().calendar()
    .buildRequest()
    .get();

```