---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0cbbfa2ea5d0694871261ed3db2f94998a4da2fadc353fba92020e7154afec54
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161681"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Extension extension = graphClient.groups("37df2ff0-0de0-4c33-8aee-75289364aef6").threads("AAQkADJizZJpEWwqDHsEpV_KA==").posts("AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=").extensions("Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate")
    .buildRequest()
    .get();

```