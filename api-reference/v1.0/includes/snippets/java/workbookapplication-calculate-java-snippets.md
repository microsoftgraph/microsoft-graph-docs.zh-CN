---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c9d4d86bbb00ebda84fdbf85e37d22c7981b42f288bc6f7899a6aab83007886
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162526"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String calculationType = "calculationType-value";

graphClient.me().drive().items("{id}").workbook().application()
    .calculate(WorkbookApplicationCalculateParameterSet
        .newBuilder()
        .withCalculationType(calculationType)
        .build())
    .buildRequest()
    .post();

```