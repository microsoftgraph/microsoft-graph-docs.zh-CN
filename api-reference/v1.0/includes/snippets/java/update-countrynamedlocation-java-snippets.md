---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c806ba706e2e05ef39421faf3b8a68d037b5900
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972050"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CountryNamedLocation namedLocation = new CountryNamedLocation();
namedLocation.displayName = "Updated named location without unknown countries and regions";
LinkedList<String> countriesAndRegionsList = new LinkedList<String>();
countriesAndRegionsList.add("CA");
countriesAndRegionsList.add("IN");
namedLocation.countriesAndRegions = countriesAndRegionsList;
namedLocation.includeUnknownCountriesAndRegions = false;

graphClient.identity().conditionalAccess().namedLocations("1c4427fd-0885-4a3d-8b23-09a899ffa959")
    .buildRequest()
    .patch(namedLocation);

```