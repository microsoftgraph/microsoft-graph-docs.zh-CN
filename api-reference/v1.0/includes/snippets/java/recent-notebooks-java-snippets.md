---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c04c8eefbc2b35188bfd768f51f1c41348c80064
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981178"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

NotebookGetRecentNotebooksCollectionPage getRecentNotebooks = graphClient.me().onenote().notebooks()
    .getRecentNotebooks(NotebookGetRecentNotebooksParameterSet
        .newBuilder()
        .withIncludePersonalNotebooks(true)
        .build())
    .buildRequest()
    .get();

```