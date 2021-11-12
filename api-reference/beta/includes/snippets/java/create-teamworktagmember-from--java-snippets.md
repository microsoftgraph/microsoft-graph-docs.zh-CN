---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 044ea89894140efe7287741c7ea795ada392233dac14d3647153f6dee6bcecf4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278270"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkTagMember teamworkTagMember = new TeamworkTagMember();
teamworkTagMember.userId = "97f62344-57dc-409c-88ad-c4af14158ff5";

graphClient.teams("53c53217-fe77-4383-bc5a-ed4937a1aecd").tags("MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==").members()
    .buildRequest()
    .post(teamworkTagMember);

```