---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4cf8dc2ec465895a926d8868e1b1e02766bcbd81
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905256"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));
requestOptions.add(new QueryOption("$search", "displayName:Android"));

IDeviceCollectionPage devices = graphClient.devices()
    .buildRequest( requestOptions )
    .get();

```