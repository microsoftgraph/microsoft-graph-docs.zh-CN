---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43c1b4addd8ac20bb2562adc964f0fdb69205855
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211667"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

DirectoryObjectCollectionWithReferencesPage members = graphClient.groups("{id}").members()
    .buildRequest( requestOptions )
    .filter("startswith(displayName, 'a')")
    .get();

```