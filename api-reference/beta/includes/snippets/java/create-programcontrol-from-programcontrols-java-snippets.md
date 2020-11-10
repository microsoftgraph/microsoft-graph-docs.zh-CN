---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f955d8e9f5e4f0f087d25f8fa2fa1af95205528e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967724"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProgramControl programControl = new ProgramControl();
programControl.controlId = "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213";
programControl.controlTypeId = "6e4f3d20-c5c3-407f-9695-8460952bcc68";
programControl.programId = "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213";

graphClient.programControls()
    .buildRequest()
    .post(programControl);

```