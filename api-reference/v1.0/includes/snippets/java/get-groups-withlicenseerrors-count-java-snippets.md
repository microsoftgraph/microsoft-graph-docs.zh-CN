---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a7787646cb348f7bebea9820b8f7ee4d5f33492d92f41c36d992b8259c7390d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219638"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

GroupCollectionPage groups = graphClient.groups()
    .buildRequest( requestOptions )
    .filter("hasMembersWithLicenseErrors eq true")
    .select("id,displayName")
    .get();

```