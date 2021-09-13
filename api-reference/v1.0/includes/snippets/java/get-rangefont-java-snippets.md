---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d0f4c713718557c243d5bd3376989fe55b1e58783b4d07b59b1e8b89febd882
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334169"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFont workbookRangeFont = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format().font()
    .buildRequest()
    .get();

```