---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13ddb50712e2b28ca09bc8be360faba5698a3a2fe02c89fb8c05ee71e5a494a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333727"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemAddress itemAddress = new ItemAddress();
itemAddress.displayName = "Home";
PhysicalAddress detail = new PhysicalAddress();
detail.type = PhysicalAddressType.HOME;
detail.postOfficeBox = null;
detail.street = "221B Baker Street";
detail.city = "London";
detail.state = null;
detail.countryOrRegion = "United Kingdom";
detail.postalCode = "E14 3TD";
itemAddress.detail = detail;

graphClient.me().profile().addresses()
    .buildRequest()
    .post(itemAddress);

```