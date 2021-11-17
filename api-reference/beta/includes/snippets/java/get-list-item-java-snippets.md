---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2392175b08b4153d8b59389cefe3335f56f6a7ba8aec11ebdaffc2a0861fa90
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103992"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("expand", "fields"));

ListItem listItem = graphClient.sites("{site-id}").lists("{list-id}").items("{item-id}")
    .buildRequest( requestOptions )
    .get();

```