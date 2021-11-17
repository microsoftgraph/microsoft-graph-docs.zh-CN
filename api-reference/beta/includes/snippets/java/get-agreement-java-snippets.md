---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1dca37a2ad0236d443732ddbb45f9fb866e7fcdca79b6a173166a4445d9565d5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902547"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Agreement agreement = graphClient.identityGovernance().termsOfUse().agreements("{id}")
    .buildRequest()
    .expand("files")
    .get();

```