---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b7b8865a2ce3a48398a46376fbc8ccf181f23feeea8bf93aa68be2ce29a4f18a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378411"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTableRow workbookTableRow = graphClient.me().drive().items("{id}").workbook().tables("{id|name}").rows("{index}")
    .buildRequest()
    .get();

```