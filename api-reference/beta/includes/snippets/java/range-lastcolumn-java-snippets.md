---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6ff0304eb9b00795892b8fd363bcadfcc1806aa3d44b1e2638e332227ff65ea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273937"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .lastColumn()
    .buildRequest()
    .get();

```