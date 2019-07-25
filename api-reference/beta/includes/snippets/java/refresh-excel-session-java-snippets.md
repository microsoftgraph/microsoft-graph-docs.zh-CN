---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0feab09a8f2966b9012561dc2f7809fe55623a4f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866493"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("workbook-session-id", "{session-id}"));

graphClient.me().drive().items("{id}").workbook()
    .refreshSession(this)
    .buildRequest( requestOptions )
    .post();

```