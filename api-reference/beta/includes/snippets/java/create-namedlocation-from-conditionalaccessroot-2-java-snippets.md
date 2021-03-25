---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f05cc8ba0d846896a8fe8eccf22ea18b991fe7e1
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208470"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CountryNamedLocation namedLocation = new CountryNamedLocation();
namedLocation.displayName = "Named location with unknown countries and regions";
LinkedList<String> countriesAndRegionsList = new LinkedList<String>();
countriesAndRegionsList.add("US");
countriesAndRegionsList.add("GB");
namedLocation.countriesAndRegions = countriesAndRegionsList;
namedLocation.includeUnknownCountriesAndRegions = true;

graphClient.identity().conditionalAccess().namedLocations()
    .buildRequest()
    .post(namedLocation);

```