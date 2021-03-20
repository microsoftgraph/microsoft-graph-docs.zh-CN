---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4338007815c8b13277f58d0810e6483d7259fe38
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947218"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IpNamedLocation namedLocation = new IpNamedLocation();
namedLocation.displayName = "Untrusted IP named location";
namedLocation.isTrusted = false;
LinkedList<IpRange> ipRangesList = new LinkedList<IpRange>();
IPv4CidrRange ipRanges = new IPv4CidrRange();
ipRanges.cidrAddress = "12.34.221.11/22";
ipRangesList.add(ipRanges);
IPv6CidrRange ipRanges1 = new IPv6CidrRange();
ipRanges1.cidrAddress = "2001:0:9d38:90d6:0:0:0:0/63";
ipRangesList.add(ipRanges1);
namedLocation.ipRanges = ipRangesList;

graphClient.identity().conditionalAccess().namedLocations()
    .buildRequest()
    .post(namedLocation);

```