---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57b5b937c73a57b9785cbdf13ee1213c3f3667c6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976496"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IpNamedLocation namedLocation = new IpNamedLocation();
namedLocation.displayName = "Untrusted named location with only IPv4 address";
namedLocation.isTrusted = false;
LinkedList<IpRange> ipRangesList = new LinkedList<IpRange>();
IPv4CidrRange ipRanges = new IPv4CidrRange();
ipRanges.cidrAddress = "6.5.4.3/18";
ipRangesList.add(ipRanges);
namedLocation.ipRanges = ipRangesList;

graphClient.identity().conditionalAccess().namedLocations("0854951d-5fc0-4eb1-b392-9b2c9d7949c2")
    .buildRequest()
    .patch(namedLocation);

```