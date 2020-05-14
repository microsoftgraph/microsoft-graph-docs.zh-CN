---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 67e7c0a38340f5cd27886ec1fbcd5c963db6d4b5
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217246"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Authorization", "Bearer {token}"));

OfferShiftRequest offerShiftRequest = new OfferShiftRequest();
offerShiftRequest.senderShiftId = "SHFT_f7e484ed-fdd6-421c-92d9-0bc9e62e2c29";
offerShiftRequest.senderMessage = "Having a family emergency, could you take this shift for me?";
offerShiftRequest.recipientUserId = "fe278b61-21ac-4872-8b41-1962bbb98e3c";

graphClient.teams("788b75d2-a911-48c0-a5e2-dc98480457e3").schedule().offerShiftRequests()
    .buildRequest( requestOptions )
    .post(offerShiftRequest);

```