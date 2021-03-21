---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c8b581712e0f4f14fe5378f732c4c18c15a6f41
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976232"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProgramControl programControl = new ProgramControl();
programControl.controlId = "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213";
programControl.controlTypeId = "6e4f3d20-c5c3-407f-9695-8460952bcc68";
programControl.programId = "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213";

graphClient.programControls()
    .buildRequest()
    .post(programControl);

```