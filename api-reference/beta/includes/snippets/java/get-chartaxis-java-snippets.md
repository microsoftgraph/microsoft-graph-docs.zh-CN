---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7baf8ef2fba62126b61911486a72e6c170bd54f6bc551ab8469a118ed0913816
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903115"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartAxis workbookChartAxis = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").axes().valueAxis()
    .buildRequest()
    .get();

```