---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2faa543a24799f9a17f6c61f7ace042e1761bc5
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870358"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").protection()
    .unprotect()
    .buildRequest()
    .post();

```