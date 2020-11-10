---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45ce0f61f03a2e0a9744d5f830c9573e02178e6d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969228"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SharedDriveItem sharedDriveItem = graphClient.shares("{shareIdOrEncodedSharingUrl}")
    .buildRequest()
    .get();

```