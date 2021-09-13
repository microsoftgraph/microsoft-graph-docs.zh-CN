---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c00b93b35afe632c55ff84f1d5ef15432d4ed47dc6ef37b13b1cc93f7b8feda3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219083"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}")
    .usedRange()
    .buildRequest()
    .get();

```