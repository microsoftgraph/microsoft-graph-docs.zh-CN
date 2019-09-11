---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6dbd360c41743a1f8edb6e74730c47af86c39fdf
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36838995"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookCommentReply workbookCommentReply = graphClient.drive().root().workbook().comments("{id}").replies("{id}")
    .buildRequest()
    .get();

```