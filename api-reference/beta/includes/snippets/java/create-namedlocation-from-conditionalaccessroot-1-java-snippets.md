---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c9430ae8cd1be740184f66d376613b52b6bd74562d070a6f997b4eb4b2e1e5ff
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220334"
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