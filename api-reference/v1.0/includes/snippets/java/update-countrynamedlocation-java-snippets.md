---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 103bb938fa0a1e3c641077d5cd47d42a7e2ed1f2a8c8fcade875cfcfcf2702ef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333533"
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