---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c18f5c1585eb4ea101355783401a1282cf5e375274390dd87ebed365fbe26f1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158531"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("expand", "fields(select=Name,Color,Quantity)"));

ListItemCollectionPage items = graphClient.sites("{site-id}").lists("{list-id}").items()
    .buildRequest( requestOptions )
    .get();

```