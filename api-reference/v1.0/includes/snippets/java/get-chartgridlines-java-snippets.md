---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd536135e7eaead56620112a9d2ee31907605e0cdc3ab6ccc85001fded4e6f4d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104623"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartGridlines workbookChartGridlines = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").axes().valueAxis().minorGridlines()
    .buildRequest()
    .get();

```