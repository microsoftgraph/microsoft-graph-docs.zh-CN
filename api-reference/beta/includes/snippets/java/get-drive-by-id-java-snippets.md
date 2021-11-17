---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09a4ac0744aca5eeea1614715397293b9ad87120541d94289b6850ce18e1a396
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105185"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Drive drive = graphClient.drives("{driveId}")
    .buildRequest()
    .get();

```