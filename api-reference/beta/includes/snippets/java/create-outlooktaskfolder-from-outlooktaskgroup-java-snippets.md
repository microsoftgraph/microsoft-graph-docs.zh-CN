---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c7769c896e279fef01155cdab820e6a113cc236
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978764"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTaskFolder outlookTaskFolder = new OutlookTaskFolder();
outlookTaskFolder.name = "Cooking";

graphClient.me().outlook().taskGroups("AAMkADIyAAAhrbe-AAA=").taskFolders()
    .buildRequest()
    .post(outlookTaskFolder);

```