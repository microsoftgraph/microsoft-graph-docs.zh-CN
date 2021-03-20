---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76c8bfe9a2a355e34dd9ec0873145918624e5da1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968206"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format()
    .autofitRows()
    .buildRequest()
    .post();

```