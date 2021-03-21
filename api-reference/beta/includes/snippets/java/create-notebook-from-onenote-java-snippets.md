---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24d85f97e1f96c473e38348f1af50bc356b523dd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978706"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Notebook notebook = new Notebook();
notebook.displayName = "Notebook name";

graphClient.me().onenote().notebooks()
    .buildRequest()
    .post(notebook);

```