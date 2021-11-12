---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1761e593e8014f4a1b06a5fae4082e354a0a39971a7b9d0f7320587d1117ee96
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162285"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartSeriesCollectionPage series = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").series()
    .buildRequest()
    .get();

```