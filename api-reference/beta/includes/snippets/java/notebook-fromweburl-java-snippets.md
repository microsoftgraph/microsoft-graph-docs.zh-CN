---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f330bf3b53c6f1f9fdf013222854b47ecb5536ed7cdc4144e3b0c78a3cb31d5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106631"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String webUrl = "webUrl value";

graphClient.me().onenote().notebooks()
    .getNotebookFromWebUrl(NotebookGetNotebookFromWebUrlParameterSet
        .newBuilder()
        .withWebUrl(webUrl)
        .build())
    .buildRequest()
    .post();

```