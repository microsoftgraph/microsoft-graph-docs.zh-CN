---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2aa125e349ad989a971b0656221e5d7738db5c0
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209067"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContractCollectionPage contracts = graphClient.contracts()
    .buildRequest()
    .get();

```