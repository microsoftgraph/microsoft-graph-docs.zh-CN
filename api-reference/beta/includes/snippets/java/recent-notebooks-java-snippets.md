---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30389d48760cee23acd214d2c90825aadc0e8cfe
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977754"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

NotebookGetrecentnotebooksCollectionPage getrecentnotebooks = graphClient.me().onenote().notebooks()
    .getrecentnotebooks(NotebookGetrecentnotebooksParameterSet
        .newBuilder()
        .withIncludePersonalNotebooks(true)
        .build())
    .buildRequest()
    .get();

```