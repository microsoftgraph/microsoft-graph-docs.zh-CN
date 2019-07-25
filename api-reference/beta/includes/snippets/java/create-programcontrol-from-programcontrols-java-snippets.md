---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f955d8e9f5e4f0f087d25f8fa2fa1af95205528e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875335"
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