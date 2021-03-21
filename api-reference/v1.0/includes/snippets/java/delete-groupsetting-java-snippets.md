---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8793ade8b1f907fc897fe666a64c9c711bdb4f45
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975229"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groupSettings("{id}")
    .buildRequest()
    .delete();

```