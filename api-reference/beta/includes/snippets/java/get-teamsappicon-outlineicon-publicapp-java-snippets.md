---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: acdf7dd4bf4e43a708ab3388c2f7ae37ff374d325cd4d52df2c4cbcc10a5b33c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218861"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppIcon teamsAppIcon = graphClient.appCatalogs().teamsApps("95de633a-083e-42f5-b444-a4295d8e9314").appDefinitions("OTVkZTYzM2EtMDgzZS00MmY1LWI0NDQtYTQyOTVkOGU5MzE0IyMxLjAuNSMjUHVibGlzaGVk").outlineIcon()
    .buildRequest()
    .get();

```