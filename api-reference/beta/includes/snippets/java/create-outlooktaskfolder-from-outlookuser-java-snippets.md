---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7371b83a744877614b1bec44b8e8924855bc4e73335e638ee3d25c7760272b44
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221309"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTaskFolder outlookTaskFolder = new OutlookTaskFolder();
outlookTaskFolder.name = "Volunteer";

graphClient.me().outlook().taskFolders()
    .buildRequest()
    .post(outlookTaskFolder);

```