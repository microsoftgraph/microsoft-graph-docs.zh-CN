---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 541b0fb5f4662747d1185070ff4ee0b8a7e2c78b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981013"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().printers("{printerId}")
    .buildRequest()
    .delete();

```