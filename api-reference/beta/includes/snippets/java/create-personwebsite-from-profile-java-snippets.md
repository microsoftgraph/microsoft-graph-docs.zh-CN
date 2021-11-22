---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a43ca6de513c79070bcd12cf488024f463c65b2856e6f16c476a463c22f8dee9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218975"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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