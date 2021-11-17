---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc12ca38a9b656dd5a42f0b2e3949369f687ead03c33608469d5687ee5bc2cb0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158501"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonInterest personInterest = new PersonInterest();
LinkedList<String> categoriesList = new LinkedList<String>();
categoriesList.add("Sports");
personInterest.categories = categoriesList;

graphClient.me().profile().interests("{id}")
    .buildRequest()
    .patch(personInterest);

```