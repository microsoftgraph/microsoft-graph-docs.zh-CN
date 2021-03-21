---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92823503a4f1eff8cb7995cc601bb241264a2b2c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972230"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFormat workbookRangeFormat = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format()
    .buildRequest()
    .get();

```