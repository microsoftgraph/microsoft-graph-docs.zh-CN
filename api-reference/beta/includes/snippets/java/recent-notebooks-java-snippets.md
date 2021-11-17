---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c04c8eefbc2b35188bfd768f51f1c41348c80064
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "61021830"
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