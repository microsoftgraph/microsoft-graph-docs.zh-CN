---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f942fdce881c7d698042b7f0ac80a1f410ff43ea
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877568"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTaskFolder outlookTaskFolder = new OutlookTaskFolder();
outlookTaskFolder.name = "Charity work";

graphClient.me().outlook().taskFolders("AAMkADIyAAAhrbPWAAA=")
    .buildRequest()
    .patch(outlookTaskFolder);

```