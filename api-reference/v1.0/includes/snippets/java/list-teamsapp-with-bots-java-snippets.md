---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 215ddf8f3b67df49983b3a0d03f1530721f188dff451ac44895d07cbe5cb1fc2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219400"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppCollectionPage teamsApps = graphClient.appCatalogs().teamsApps()
    .buildRequest()
    .filter("appDefinitions/any(a:a/bot ne null)")
    .expand("appDefinitions($expand=bot)")
    .get();

```