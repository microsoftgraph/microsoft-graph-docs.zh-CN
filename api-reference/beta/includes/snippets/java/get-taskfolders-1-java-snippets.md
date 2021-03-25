---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69f15ecfd8b70016a72b428065201e3395dd162a
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210480"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTaskFolderCollectionPage taskFolders = graphClient.me().outlook().taskGroups("AAMkADIyAAAhrbe-AAA=").taskFolders()
    .buildRequest()
    .get();

```