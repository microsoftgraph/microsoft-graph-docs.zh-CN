---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 11552d19c03bfb30812e88ef0b9dfe4018122902
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979632"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().printers("{id}")
    .buildRequest()
    .delete();

```