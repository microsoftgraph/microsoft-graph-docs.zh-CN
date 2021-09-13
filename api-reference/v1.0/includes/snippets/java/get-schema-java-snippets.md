---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2454b9213eb805fa775f1691c622c4dc9f408adfc5c1095c1f4147c1a0a90858
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409052"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Schema schema = graphClient.connections("contosohr").schema()
    .buildRequest()
    .get();

```