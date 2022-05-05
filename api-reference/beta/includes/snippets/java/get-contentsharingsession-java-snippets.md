---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5aecb953e9268697d4f29d91154cc0c02b79ad60
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210364"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContentSharingSession contentSharingSession = graphClient.communications().calls("7531d31f-d10d-44de-802f-c569dbca451c").contentSharingSessions("7e1b4346-85a6-4bdd-abe3-d11c5d420efe")
    .buildRequest()
    .get();

```