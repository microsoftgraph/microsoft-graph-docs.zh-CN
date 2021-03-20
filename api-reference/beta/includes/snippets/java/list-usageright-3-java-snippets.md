---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f6d1ee965a7e006ee6be2c2d629ca4188ee05fb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942030"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUsageRightCollectionPage usageRights = graphClient.users("{userId}").usageRights()
    .buildRequest()
    .get();

```