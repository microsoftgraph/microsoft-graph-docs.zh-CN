---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29880f003b02a5c0889951bdaa9d7a0bc7a72fb8d91d5b0229459949bb6c6f62
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218713"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=minimal"));

OrgContactDeltaCollectionPage delta = graphClient.contacts()
    .delta()
    .buildRequest( requestOptions )
    .select("displayName,jobTitle,mail")
    .get();

```