---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74ecd5bea662f3bd5cf0c7b94610bbe8769d02b70250e7878646f7f98703926b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378708"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookTable workbookTable = graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .buildRequest()
    .get();

```