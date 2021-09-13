---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 097e5ce50d2009dd17090820f7384d7bc98908b68486913cf8313db4129ab20d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105358"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("select", "id,name,lastModifiedDateTime"));
requestOptions.add(new QueryOption("expand", "columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))"));

List list = graphClient.sites("{site-id}").lists("{list-id}")
    .buildRequest( requestOptions )
    .get();

```