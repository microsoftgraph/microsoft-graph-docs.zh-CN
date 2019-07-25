---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2c05884129b85849da53acc227132cf85a1d6b72
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869713"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("$filter", "id eq 'String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color')"));

Message message = graphClient.me().messages("AAMkAGE1M2_bs88AACHsLqWAAA=")
    .buildRequest( requestOptions )
    .expand("singleValueExtendedProperties($filter=id%20eq%20'String%20%7B66f5a359-4659-4830-9070-00047ec6ac6e%7D%20Name%20Color')")
    .get();

```