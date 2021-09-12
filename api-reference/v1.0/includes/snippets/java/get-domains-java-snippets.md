---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c42348ca67c16d4e7dfcb0744262f1e8d68671701890cb720dfd0b1b1953c6d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163285"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DomainCollectionPage domains = graphClient.domains()
    .buildRequest()
    .get();

```