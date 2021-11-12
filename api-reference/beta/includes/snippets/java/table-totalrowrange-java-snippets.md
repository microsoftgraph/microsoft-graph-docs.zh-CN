---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 096287c4a1b51ce10764e5958ee7605271b271400104d2bc0574b487ee083a1f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903039"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .totalRowRange()
    .buildRequest()
    .get();

```