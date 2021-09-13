---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d04e28b26ebfbeabb5ede3d5857e4d0a45829884196a161788106b36068c589f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409297"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookCommentCollectionPage comments = graphClient.drive().items("{id}").workbook().comments()
    .buildRequest()
    .get();

```