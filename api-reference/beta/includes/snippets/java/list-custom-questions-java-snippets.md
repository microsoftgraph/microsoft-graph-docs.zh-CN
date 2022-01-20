---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fa6490543785399c4fb34c8a4ac7265b1c2d702b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113191"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MeetingRegistrationQuestionCollectionPage customQuestions = graphClient.me().onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ").registration().microsoft.graph.meetingRegistration().customQuestions()
    .buildRequest()
    .get();

```