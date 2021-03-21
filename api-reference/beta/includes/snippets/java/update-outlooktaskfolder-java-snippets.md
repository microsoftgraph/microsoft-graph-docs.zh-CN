---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a2061dea7c94dae503594a55d6de80be19ca449
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982598"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTaskFolder outlookTaskFolder = new OutlookTaskFolder();
outlookTaskFolder.name = "Charity work";

graphClient.me().outlook().taskFolders("AAMkADIyAAAhrbPWAAA=")
    .buildRequest()
    .patch(outlookTaskFolder);

```