---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3640f1c85515fc31728275563365bbe00772c78433681aea9c8bae970bfcd350
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277616"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11021").assignments("19002")
    .publish()
    .buildRequest()
    .post();

```