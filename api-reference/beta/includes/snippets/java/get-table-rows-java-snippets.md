---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3641eced806cdd1869fdf3948bfbcf9b1f008c49f391d066e670504a6e476b5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219849"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTableRowCollectionPage rows = graphClient.me().drive().items("{id}").workbook().tables("{id|name}").rows()
    .buildRequest()
    .skip(5)
    .top(5)
    .get();

```