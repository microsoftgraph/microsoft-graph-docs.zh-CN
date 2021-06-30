---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8492225db53a037ccd2283ffb9eba41420c96d8
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210252"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkTag teamworkTag = graphClient.teams("53c53217-fe77-4383-bc5a-ed4937a1aecd").tags("MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==")
    .buildRequest()
    .get();

```