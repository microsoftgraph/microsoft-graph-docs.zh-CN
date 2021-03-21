---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fadfee4d05f15cff94d2ec922aa07c3833dc5deb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980533"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String name = "name-value";

graphClient.me().drive().items("{id}").workbook().worksheets()
    .add(WorkbookWorksheetAddParameterSet
        .newBuilder()
        .withName(name)
        .build())
    .buildRequest()
    .post();

```