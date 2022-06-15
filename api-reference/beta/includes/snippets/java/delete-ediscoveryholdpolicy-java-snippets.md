---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e39a8562e1b456e91252e4b3424e23850068b8ce
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092498"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.security().cases().ediscoveryCases("b0073e4e-4184-41c6-9eb7-8c8cc3e2288b").legalHolds("a4d3421d-b756-47ac-ad43-5d587c5dfe75")
    .buildRequest()
    .delete();

```