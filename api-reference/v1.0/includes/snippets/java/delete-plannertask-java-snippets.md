---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3a7cbd1ecf09ebb598601cc3bbc669c93fc0291bc28a54e43609c36aa56c4ac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278513"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("If-Match", "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""));

graphClient.planner().tasks("{id}")
    .buildRequest( requestOptions )
    .delete();

```