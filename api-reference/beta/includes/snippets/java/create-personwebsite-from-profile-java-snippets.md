---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04ea0f75445fecdfca59d4a2b7f9ff5e1f80373f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980873"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonWebsite personWebsite = new PersonWebsite();
LinkedList<String> categoriesList = new LinkedList<String>();
categoriesList.add("football");
personWebsite.categories = categoriesList;
personWebsite.displayName = "Lyn Damer";
personWebsite.webUrl = "www.lyndamer.no";

graphClient.me().profile().websites()
    .buildRequest()
    .post(personWebsite);

```