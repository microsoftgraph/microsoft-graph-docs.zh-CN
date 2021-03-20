---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3d6a35af4161f78293d1887832605f26d0c8fe2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970211"
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