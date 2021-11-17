---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d851903a4ee99ad74562694f3742eb2931140d076b05f33f04e617fa4a26f0e0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278450"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("If-Match", "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""));

graphClient.planner().buckets("{id}")
    .buildRequest( requestOptions )
    .delete();

```