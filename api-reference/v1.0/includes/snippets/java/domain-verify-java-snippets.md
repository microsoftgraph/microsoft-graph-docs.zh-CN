---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 530f564b00e854d0d033839e80e0b63bfb4a83d3d06e520728e4355b17ebddac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107067"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.domains("{domain-name}")
    .verify()
    .buildRequest()
    .post();

```