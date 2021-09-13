---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72744a8b8f24c0ff3e53a5fe9c728be1b7079bb38a7ccff3c454c50584b6ee87
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902945"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeSort workbookRangeSort = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().sort()
    .buildRequest()
    .get();

```