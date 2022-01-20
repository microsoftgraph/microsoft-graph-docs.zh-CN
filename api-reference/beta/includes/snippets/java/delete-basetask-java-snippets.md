---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1be98f7f7a26752e5e92757ad2ccde1ad5300223
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116662"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().tasks().lists("AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAu").tasks("AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AkOO4xOT")
    .buildRequest()
    .delete();

```