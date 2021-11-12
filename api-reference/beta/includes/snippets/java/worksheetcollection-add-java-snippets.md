---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29b04b57b46ca9d08a23f3cb1f033db8dd62e0290248a2e5811b1a5e38b544b1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106582"
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