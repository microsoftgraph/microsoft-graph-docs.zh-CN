---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81fce431d3e7c4f89e4aa8089edf2bfcd09af515ac0994b48716da5a8952b5c2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162253"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11021").assignments("19002").submissions("850f51b7")
    .return()
    .buildRequest()
    .post();

```