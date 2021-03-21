---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1bd09a6c4fc15ef6bd1bc756515952959fa64b28
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983405"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTableColumnCollectionPage columns = graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns()
    .buildRequest()
    .skip(5)
    .top(5)
    .get();

```