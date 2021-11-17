---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c227da9e729a1285f3106cbad554b58b2c2458e9039cf8b0b30478e85ca3faa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220079"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProgramCollectionPage programs = graphClient.programs()
    .buildRequest()
    .get();

```