---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e3531c1421070424c788cf5f86f527804c93c4f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978073"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonInterest personInterest = new PersonInterest();
LinkedList<String> categoriesList = new LinkedList<String>();
categoriesList.add("Sports");
personInterest.categories = categoriesList;
personInterest.description = "World's greatest football club";
personInterest.displayName = "Chelsea FC";
personInterest.webUrl = "https://www.chelseafc.com";

graphClient.me().profile().interests()
    .buildRequest()
    .post(personInterest);

```