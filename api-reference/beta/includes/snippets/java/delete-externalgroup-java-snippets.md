---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13be9c064942009ba99a9bc036207adcdf3c0ce4c2e37367da8740f1fb929134
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278783"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.external().connections("contosohr").groups("31bea3d537902000")
    .buildRequest()
    .delete();

```