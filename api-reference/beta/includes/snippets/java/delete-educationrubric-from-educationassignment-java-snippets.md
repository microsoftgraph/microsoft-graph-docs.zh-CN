---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20b9e8103406d25745ed08233e90e2a8525b54b8771fb7a132494f83789b4b94
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332507"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("{id}").assignments("{id}").rubric().reference()
    .buildRequest()
    .delete();

```