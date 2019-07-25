---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9ad576c00d64c5178bc883aca797aa092a0c0a65
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862895"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPostCollectionPage posts = graphClient.groups("0d75b8dc-c42d-44dd-890a-751a99c0589f").threads("AAQkAD8EJUmcWwTJi06Cew==").posts()
    .buildRequest()
    .get();

```