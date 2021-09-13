---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1da8e48d3627cce050568899fd30ea7c3cfc5520a4d3e4b8ebfc7136da1be198
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221149"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .lastRow()
    .buildRequest()
    .get();

```