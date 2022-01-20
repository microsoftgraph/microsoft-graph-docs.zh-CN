---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 924d34e3d1533aaedeb7a587ff4a41fc613dcc31e7f28a1f5dd4851fbf645364
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219548"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.external().connections("contosohr").groups("31bea3d537902000").members("14m1b9c38qe647f6a")
    .buildRequest()
    .delete();

```