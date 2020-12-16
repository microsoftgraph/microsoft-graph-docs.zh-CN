---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23afe16a617cdef361d27b42c122b015de2a79e9
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690337"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITeamsAppCollectionPage teamsApps = graphClient.appCatalogs().teamsApps()
    .buildRequest()
    .filter("externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'")
    .get();

```