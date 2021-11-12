---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: adf4cca9984892824933aeecddf5bec24c2352b92d6eaa6491f5dd1c27787108
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219723"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerTaskCollectionPage tasks = graphClient.planner().buckets("gcrYAaAkgU2EQUvpkNNXLGQAGTtu").tasks()
    .buildRequest()
    .get();

```