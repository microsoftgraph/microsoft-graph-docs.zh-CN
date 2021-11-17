---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23ee2700e29b7e21862063019609de3ca8decff50671e3d1216acbbf6d524b55
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103793"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=minimal"));

UserDeltaCollectionPage delta = graphClient.users()
    .delta()
    .buildRequest( requestOptions )
    .select("displayName,jobTitle,mobilePhone")
    .get();

```