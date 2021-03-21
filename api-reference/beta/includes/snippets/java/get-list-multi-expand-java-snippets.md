---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c87029b69af5d4223141556bef6d3a802c5ad99a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958019"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("select", "name,lastModifiedDateTime"));
requestOptions.add(new QueryOption("expand", "columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))"));

List list = graphClient.sites("{site-id}").lists("{list-id}")
    .buildRequest( requestOptions )
    .get();

```