---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a743cdd0237ace93344aafcbba637767b23db44
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978919"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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