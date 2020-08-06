---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e55598fb1528d623b0b26fb14976574b06184e7
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566022"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("$filter", "microsoft.graph.countryNamedLocation/countriesAndRegions/any(c: c eq 'CA')"));

INamedLocationCollectionPage namedLocations = graphClient.identity().conditionalAccess().namedLocations()
    .buildRequest( requestOptions )
    .get();

```