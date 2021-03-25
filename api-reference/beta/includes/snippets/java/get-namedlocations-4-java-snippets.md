---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b14bb208fa6cbce16cf6ead0dfd1c70ac35eeda7
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209236"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

NamedLocationCollectionPage namedLocations = graphClient.identity().conditionalAccess().namedLocations()
    .buildRequest()
    .filter("microsoft.graph.countryNamedLocation/countriesAndRegions/any(c: c eq 'CA')")
    .get();

```