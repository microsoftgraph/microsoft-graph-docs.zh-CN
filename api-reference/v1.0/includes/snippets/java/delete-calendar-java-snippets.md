---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc13f7ee6db62a9118c3fd9b2b41fc2112aedaee
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969479"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().calendar()
    .buildRequest()
    .delete();

```