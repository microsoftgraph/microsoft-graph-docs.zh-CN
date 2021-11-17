---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad39772d67eb1c04301840db22ee8457b55e5a8c3f53a9fa4f41a832c24d0c3c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218862"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppIcon teamsAppIcon = graphClient.appCatalogs().teamsApps("5a31d4f7-a11d-4052-96eb-1b40786a2a78").appDefinitions("NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk").colorIcon()
    .buildRequest()
    .get();

```