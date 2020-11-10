---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba7093fe0a27585ae3a400c6be79c7bf9432bada
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982048"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISecureScoreControlProfileCollectionPage secureScoreControlProfiles = graphClient.security().secureScoreControlProfiles()
    .buildRequest()
    .get();

```