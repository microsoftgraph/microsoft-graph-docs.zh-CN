---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aea375bb625bc1fc79c8fe7853756e905499e359
ms.sourcegitcommit: 3834b7b0287ee71668c52c42d3465ca19366e678
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2020
ms.locfileid: "43082167"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=minimal"));

OrgContact orgContact = graphClient.contacts("delta")
    .buildRequest( requestOptions )
    .select("displayName,jobTitle,mail")
    .get();

```