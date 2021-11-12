---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10f8796f9dad65bbe1fd1ebdad87d0113d5f8245c7d4e983b23dba8cbcc8343e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220338"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartTitle workbookChartTitle = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").title()
    .buildRequest()
    .get();

```