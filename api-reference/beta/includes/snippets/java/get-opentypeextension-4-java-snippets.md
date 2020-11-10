---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5dc8fed9d8f7218eda791f4d58077afcb4a308b0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975664"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Extension extension = graphClient.groups("37df2ff0-0de0-4c33-8aee-75289364aef6").threads("AAQkADJizZJpEWwqDHsEpV_KA==").posts("AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=").extensions("Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate")
    .buildRequest()
    .get();

```