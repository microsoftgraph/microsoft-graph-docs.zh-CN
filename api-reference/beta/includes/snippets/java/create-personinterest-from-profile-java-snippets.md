---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 343e98ddebfa61e1ed67c1c2d9dee47de15d12c3b01f4075e34093fcacf9e13d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279591"
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