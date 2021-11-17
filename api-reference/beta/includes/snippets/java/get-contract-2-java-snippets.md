---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c61607b05dcb6cb460941e88ec991ab16c5af27cc554e34a1ef166a71e5183a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902428"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContractCollectionPage contracts = graphClient.contracts()
    .buildRequest()
    .get();

```