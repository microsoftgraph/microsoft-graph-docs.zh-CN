---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8c8fc1aec87b2ece7495910686e5c5eb1a2e864
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208591"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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