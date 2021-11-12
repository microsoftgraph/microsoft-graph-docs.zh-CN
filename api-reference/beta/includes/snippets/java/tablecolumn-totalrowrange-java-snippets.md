---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af58e44f7ea0493bc83e7ae6e141e9d5ce74a79bdc3c2055641c0ddbeb48338d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333389"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns("{id|name}")
    .totalRowRange()
    .buildRequest()
    .get();

```