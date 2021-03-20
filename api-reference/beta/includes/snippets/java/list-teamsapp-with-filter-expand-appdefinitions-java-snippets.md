---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b02740c435782d553cf049e7962a7298c47e687f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966894"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppCollectionPage teamsApps = graphClient.appCatalogs().teamsApps()
    .buildRequest()
    .filter("id eq '876df28f-2e78-423b-94a5-44181bd0e225'")
    .expand("appDefinitions")
    .get();

```