---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 069c87fd3479938992d45a5b93a50a908bc51f3afacfb489307918efe8b5f23d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334108"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("expand", "fields"));

ListItemVersion listItemVersion = graphClient.sites("{site-id}").lists("{list-id}").items("{item-id}").versions("{version-id}")
    .buildRequest( requestOptions )
    .get();

```