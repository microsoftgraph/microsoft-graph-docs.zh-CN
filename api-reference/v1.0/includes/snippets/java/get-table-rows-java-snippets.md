---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 093bb3e0ccbd0ca165e3f7330a3c48eabeef3cc2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884814"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("$skip", "5"));

IWorkbookTableRowCollectionPage rows = graphClient.me().drive().items("{id}").workbook().tables("{id|name}").rows()
    .buildRequest( requestOptions )
    .top(5)
    .get();

```