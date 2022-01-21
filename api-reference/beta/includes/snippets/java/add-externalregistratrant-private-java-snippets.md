---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c251e66752ea6741034abe5ac2328384d739f29
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118894"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalMeetingRegistrant meetingRegistrantBase = new ExternalMeetingRegistrant();
meetingRegistrantBase.id = "30494ab7-7338-4592-bfec-a4333be2a0a6";
meetingRegistrantBase.tenantId = "909c6581-5130-43e9-88f3-fcb3582cde37";
meetingRegistrantBase.userId = "cc515404-b55c-466e-b896-992c918ecc01";

graphClient.me().onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ").registration().registrants()
    .buildRequest()
    .post(meetingRegistrantBase);

```