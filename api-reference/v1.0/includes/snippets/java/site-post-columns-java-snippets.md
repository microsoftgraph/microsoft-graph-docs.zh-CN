---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9937668bd3489b06480f1ec8e9f100efe5d0aacd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59130158"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ColumnDefinition columnDefinition = new ColumnDefinition();
columnDefinition.description = "test";
columnDefinition.enforceUniqueValues = false;
columnDefinition.hidden = false;
columnDefinition.indexed = false;
columnDefinition.name = "Title";
TextColumn text = new TextColumn();
text.allowMultipleLines = false;
text.appendChangesToExistingText = false;
text.linesForEditing = 0;
text.maxLength = 255;
columnDefinition.text = text;

graphClient.sites("{site-id}").columns()
    .buildRequest()
    .post(columnDefinition);

```