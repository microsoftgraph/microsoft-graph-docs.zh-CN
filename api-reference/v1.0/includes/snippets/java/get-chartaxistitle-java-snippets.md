---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 77df3da357388119370b85ba745313323bfcd3b4b7193ccb270e8bf20771bbd9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104341"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartAxisTitle workbookChartAxisTitle = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").axes().valueAxis().title()
    .buildRequest()
    .get();

```