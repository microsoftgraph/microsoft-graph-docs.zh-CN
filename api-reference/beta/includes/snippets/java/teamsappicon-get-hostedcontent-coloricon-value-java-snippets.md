---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5acd2d579c41d3d4843184de7a9a4170c3d84361c9e268385bb7b0c2d0d49174
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218852"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkHostedContent teamworkHostedContent = graphClient.appCatalogs().teamsApps("5a31d4f7-a11d-4052-96eb-1b40786a2a78").appDefinitions("NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk").colorIcon().hostedContent()
    .buildRequest()
    .get();

```