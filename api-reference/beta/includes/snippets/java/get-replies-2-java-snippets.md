---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69486895596376a59b2e368f1f70601ea73447eb
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209409"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookCommentReplyCollectionPage replies = graphClient.drive().items("{id}").workbook().comments("{id}").replies()
    .buildRequest()
    .get();

```