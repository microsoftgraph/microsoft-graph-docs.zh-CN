---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ab7c93ec3ec553a0b2280d2148ac82821126a62d9b538f19f0ba3042de49145
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278501"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartPoint workbookChartPoint = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").series("{undefined}").points("{undefined}")
    .buildRequest()
    .get();

```