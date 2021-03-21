---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19ffa4ce7487370f1eafa66b74cb6c1ad7074c4a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970952"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{item-id}")
    .buildRequest()
    .delete();

```