---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0ddd57610a1eaf522a7e5850022b58bb45a9dc7f87c389c834eed3243eaec0e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162173"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkTag teamworkTag = new TeamworkTag();
teamworkTag.displayName = "Finance";

graphClient.teams("53c53217-fe77-4383-bc5a-ed4937a1aecd").tags("MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==")
    .buildRequest()
    .patch(teamworkTag);

```