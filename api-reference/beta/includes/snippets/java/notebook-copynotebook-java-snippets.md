---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25f4174ca836ee3061fdf5006449da39f1ab5c6f68ec9f4d4375700dd5fc7c8b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220092"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String groupId = "groupId-value";

String renameAs = "renameAs-value";

graphClient.me().onenote().notebooks("{id}")
    .copyNotebook(NotebookCopyNotebookParameterSet
        .newBuilder()
        .withGroupId(groupId)
        .withRenameAs(renameAs)
        .withNotebookFolder(null)
        .withSiteCollectionId(null)
        .withSiteId(null)
        .build())
    .buildRequest()
    .post();

```