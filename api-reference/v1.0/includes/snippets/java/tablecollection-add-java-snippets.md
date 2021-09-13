---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a86896e774d7c29669636c27e761cbf22ca8b61a83f85a3a09ca200ac2e1f3a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105908"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String address = "Sheet1!A1:D5";

Boolean hasHeaders = true;

graphClient.me().drive().items("{id}").workbook().tables()
    .add(WorkbookTableAddParameterSet
        .newBuilder()
        .withAddress(address)
        .withHasHeaders(hasHeaders)
        .build())
    .buildRequest()
    .post();

```