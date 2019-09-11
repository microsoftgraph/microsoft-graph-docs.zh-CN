---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 24cc1b59a75a2102ad766b5f2ebdf07b6f6c32bc
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36839036"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IWorkbookCommentReplyCollectionPage replies = graphClient.drive().root().workbook().comments("{id}").replies()
    .buildRequest()
    .get();

```