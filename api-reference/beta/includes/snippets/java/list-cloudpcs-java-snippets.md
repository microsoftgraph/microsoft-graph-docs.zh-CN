---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c89244ef27702aad960868e0d5d4a46b742f436b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973567"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPCCollectionPage cloudPCs = graphClient.deviceManagement().virtualEndpoint().cloudPCs()
    .buildRequest()
    .get();

```