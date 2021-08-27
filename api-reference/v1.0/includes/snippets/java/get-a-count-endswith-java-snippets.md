---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c541e1d922ea3e83ce14f05dc034bd9b42bb2f32931ab5cf8c1aa6fad99f9530
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409664"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

UserCollectionPage users = graphClient.users()
    .buildRequest( requestOptions )
    .filter("endswith(mail,'a@contoso.com')")
    .orderBy("userPrincipalName")
    .get();

```