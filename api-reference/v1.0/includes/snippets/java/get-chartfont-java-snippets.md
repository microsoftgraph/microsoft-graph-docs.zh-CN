---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93699981a67f117205a055f616c30454d7f92f3ea98104182e898183fc7c2850
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106044"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartFont workbookChartFont = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").axes().valueAxis().format().font()
    .buildRequest()
    .get();

```