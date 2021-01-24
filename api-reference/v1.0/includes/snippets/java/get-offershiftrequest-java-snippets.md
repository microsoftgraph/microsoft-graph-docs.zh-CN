---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 933853bcce5c8c761de0511b81e80a33688ede1a
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946349"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOfferShiftRequestCollectionPage offerShiftRequests = graphClient.teams("{teamId}").schedule().offerShiftRequests()
    .buildRequest()
    .get();

```