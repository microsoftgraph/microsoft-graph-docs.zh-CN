---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5720c68bd4844b9d2b1545fec4a8d551840c2913fae7138b0c1ca8ec81e09f52
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218486"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Notebook notebook = new Notebook();
notebook.displayName = "My Private notebook";

graphClient.me().onenote().notebooks()
    .buildRequest()
    .post(notebook);

```