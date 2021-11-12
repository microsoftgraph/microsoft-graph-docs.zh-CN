---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7fedc7084ef8730c817e2f3f5abdb5f3b82e319b05915c90ff63ed508f09dbc7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218912"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTaskGroup outlookTaskGroup = new OutlookTaskGroup();
outlookTaskGroup.name = "Leisure tasks";

graphClient.me().outlook().taskGroups()
    .buildRequest()
    .post(outlookTaskGroup);

```