---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f06ce696f33f3da096dbbcd3a840a232df1e46e0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977973"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().b2xUserFlows("{id}")
    .buildRequest()
    .delete();

```