---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 667dc1cdde70dfdeda2ad7e7cdaecdf9cb6096b16e9922fe38770494d392c581
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219215"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

int int32 = graphClient.groups("{id}").transitiveMembers().count()
    .buildRequest( requestOptions )
    .get();

```