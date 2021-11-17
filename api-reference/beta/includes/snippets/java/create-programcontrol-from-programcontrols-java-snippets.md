---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da5a00345af738880dd162d0f158db90ce467d28f41921e3cac354d74a15fd74
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333327"
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