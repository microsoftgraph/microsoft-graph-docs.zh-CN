---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a1f9a5c0d0e5ece3532804e491c14356a3b7927
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50984232"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppCollectionPage teamsApps = graphClient.appCatalogs().teamsApps()
    .buildRequest()
    .filter("externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'")
    .get();

```