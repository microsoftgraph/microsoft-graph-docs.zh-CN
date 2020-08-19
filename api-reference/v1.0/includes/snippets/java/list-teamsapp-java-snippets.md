---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a0a494bf3c9e8a1f91976dfbc9e902224e3e48f
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808977"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("$filter", "id eq 'b1c5353a-7aca-41b3-830f-27d5218fe0e5'"));

ITeamsAppCollectionPage teamsApps = graphClient.appCatalogs().teamsApps()
    .buildRequest( requestOptions )
    .get();

```