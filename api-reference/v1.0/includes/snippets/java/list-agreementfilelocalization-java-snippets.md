---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3aada860d8c57c29eeab46728291a2f5eacb9e08
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63515865"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Agreement agreement = graphClient.identityGovernance().termsOfUse().agreements("94410bbf-3d3e-4683-8149-f034e55c39dd")
    .buildRequest()
    .expand("files")
    .get();

```