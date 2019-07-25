---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7baebca280b162f001931666c5d9271f715c9da2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888336"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("select", "id,name,lastModifiedDateTime"));
requestOptions.add(new QueryOption("expand", "columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))"));

List list = graphClient.sites("{site-id}").lists("{list-id}")
    .buildRequest( requestOptions )
    .get();

```