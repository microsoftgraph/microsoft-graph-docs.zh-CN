---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 87609af54e1f862d6505c2a06123357603904729f3883b04a7d47ebc39a24178
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104058"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppCollectionPage teamsApps = graphClient.appCatalogs().teamsApps()
    .buildRequest()
    .filter("externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'")
    .get();

```