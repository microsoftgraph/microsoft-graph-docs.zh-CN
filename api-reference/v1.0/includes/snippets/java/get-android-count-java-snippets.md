---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e45bb3e16599f140674ca9f1a319ec515d2bcb589ea42bc4a1278d9b3e9e78c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333985"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));
requestOptions.add(new QueryOption("$search", "displayName:Android"));

DeviceCollectionPage devices = graphClient.devices()
    .buildRequest( requestOptions )
    .get();

```