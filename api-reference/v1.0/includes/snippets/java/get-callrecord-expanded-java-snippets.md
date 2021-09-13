---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 352828062fd9250f6d56fcc68acb33451f706e8ceaa345f6078c1f8ffe266e2b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220034"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CallRecord callRecord = graphClient.communications().callRecords("{id}")
    .buildRequest()
    .expand("sessions($expand=segments)")
    .get();

```