---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b733567e20736e611df4f84c68ff939ab0527fe1
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393653"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupCollectionPage groups = graphClient.groups()
    .buildRequest()
    .filter("assignedLicenses/any()")
    .select("id,assignedLicenses")
    .get();

```