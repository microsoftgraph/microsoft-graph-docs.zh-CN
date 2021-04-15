---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 557db77474f099ca7b4d7c060d870b2ca0745fac
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51765963"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppCollectionPage teamsApps = graphClient.appCatalogs().teamsApps()
    .buildRequest()
    .filter("appDefinitions/any(a:a/allowedInstallationScopes has 'personal')")
    .expand("appDefinitions($select=id,displayName,allowedInstallationScopes)")
    .get();

```