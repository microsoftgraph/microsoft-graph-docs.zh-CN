---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e3bf22c610070ad8ff6fc5827d25dbebd123338
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971603"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .clearFilters()
    .buildRequest()
    .post();

```