---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a28be6fdf4ea6dd0ca531d3a6d0dbadec76fde3
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692888"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserCollectionWithReferencesPage allowedUsers = graphClient.print().shares("{id}").allowedUsers()
    .buildRequest()
    .get();

```