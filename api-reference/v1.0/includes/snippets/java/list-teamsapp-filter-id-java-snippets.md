---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 769e561b288ffcb100a76a9217c168c37a5defa7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979217"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppCollectionPage teamsApps = graphClient.appCatalogs().teamsApps()
    .buildRequest()
    .filter("id eq 'b1c5353a-7aca-41b3-830f-27d5218fe0e5'")
    .get();

```