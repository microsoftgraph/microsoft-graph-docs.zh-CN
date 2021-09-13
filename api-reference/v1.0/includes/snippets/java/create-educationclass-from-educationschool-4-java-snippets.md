---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7fa04165bdb1f972cf8c834e66a576740ec985abf6a467f76dfc4da2fac874a5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101331"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().schools("{school-id}").users("{user-id}")
    .buildRequest()
    .delete();

```