---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b6908520e3a3c904205461e05f4676ef41f74035
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878142"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Extension extension = new Extension();
extension.additionalDataManager().put("@odata.type", new JsonPrimitive("#microsoft.outlookServices.openTypeExtension"));
extension.extensionName = "Com.Contoso.Estimate";
extension.companyName = "Contoso";
extension.expirationDate = "2016-07-30T11:00:00Z";
extension.DealValue = 1010100;
LinkedList<String> topPicksList = new LinkedList<String>();
topPicksList.add("Employees only");
topPicksList.add("Add spouse or guest");
topPicksList.add("Add family");
extension.topPicks = topPicksList;

graphClient.groups("37df2ff0-0de0-4c33-8aee-75289364aef6").threads("AAQkADJizZJpEWwqDHsEpV_KA==").posts("AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=").extensions("Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate")
    .buildRequest()
    .patch(extension);

```