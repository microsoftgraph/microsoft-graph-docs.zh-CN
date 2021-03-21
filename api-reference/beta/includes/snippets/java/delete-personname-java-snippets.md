---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a45f593d9cd3f9482e78f9bdaccaf4d319b33bbb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980799"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().names("{id}")
    .buildRequest()
    .delete();

```