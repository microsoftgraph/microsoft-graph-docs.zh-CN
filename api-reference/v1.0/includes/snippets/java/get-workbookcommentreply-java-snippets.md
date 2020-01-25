---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f100fd7b03b1bf5132c041df1ae3962e6afb3448
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41493869"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookCommentReply workbookCommentReply = graphClient.drive().items("{id}").workbook().comments("{id}").replies("{id}")
    .buildRequest()
    .get();

```