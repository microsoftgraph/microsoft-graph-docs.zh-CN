---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ebafe338044cb6f278660868361a8ebc0c619329abacd9be8396562e739a54e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161850"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTaskDefinition printTaskDefinition = graphClient.print().taskDefinitions("fab143fd-ee61-4358-8558-2c7dee953982")
    .buildRequest()
    .get();

```