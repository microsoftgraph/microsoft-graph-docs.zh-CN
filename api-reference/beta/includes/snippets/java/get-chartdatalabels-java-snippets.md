---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62b87bbdeba767b65643a0a517ff801bc63648b501b9a62f354705b33f1fc027
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101422"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartDataLabels workbookChartDataLabels = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").dataLabels()
    .buildRequest()
    .get();

```