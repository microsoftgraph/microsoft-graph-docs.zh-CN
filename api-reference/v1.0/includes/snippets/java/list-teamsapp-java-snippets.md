---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af21757a1dcab99b9f58caa11e79c0accb877ef8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983342"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITeamsAppCollectionPage teamsApps = graphClient.appCatalogs().teamsApps()
    .buildRequest()
    .filter("id eq 'b1c5353a-7aca-41b3-830f-27d5218fe0e5'")
    .get();

```