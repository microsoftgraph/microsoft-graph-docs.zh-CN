---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97cf079b65470c6b82f9dd63276d77c4c00f3467
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978020"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("expand", "fields(select=Name,Color,Quantity)"));

ListItemCollectionPage items = graphClient.sites("{site-id}").lists("{list-id}").items()
    .buildRequest( requestOptions )
    .get();

```