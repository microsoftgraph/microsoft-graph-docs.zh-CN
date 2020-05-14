---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ea6cc3153b0b884168aa42ea078f2d86c0dcf33
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "43511115"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "Updating the latest guidelines";

graphClient.drives("{drive-id}").items("{item-id}")
    .checkin(null,comment)
    .buildRequest()
    .post();

```