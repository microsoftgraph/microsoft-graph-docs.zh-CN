---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 05ad6de671d8280a82a38c18fcff1f752e879778
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878357"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Extension extension = new Extension();
extension.additionalDataManager().put("@odata.type", new JsonPrimitive("microsoft.graph.openTypeExtension"));
extension.extensionName = "Com.Contoso.Deal";
extension.companyName = "Alpine Skis";
extension.dealValue = 1010100;
extension.expirationDate = "2015-07-03T13:04:00Z";

graphClient.groups("f5480dfd-7d77-4d0b-ba2e-3391953cc74a").events("AAMkADVl17IsAAA=").extensions()
    .buildRequest()
    .post(extension);

```