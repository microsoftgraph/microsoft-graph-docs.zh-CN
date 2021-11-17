---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 890ec9382fa34563182abb0eaeef5c06d4c14dc2de099e559cdc4dc5a056b81b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218495"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().classes("11014").assignmentCategories("19002")
    .buildRequest()
    .delete();

```