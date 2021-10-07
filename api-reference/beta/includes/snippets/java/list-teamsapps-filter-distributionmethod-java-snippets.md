---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5faed4999f52f0923bb762658a262e5ae117afe502ec971ccbf645583d19d2b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215713"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppCollectionPage teamsApps = graphClient.appCatalogs().teamsApps()
    .buildRequest()
    .filter("distributionMethod eq 'organization'")
    .get();

```