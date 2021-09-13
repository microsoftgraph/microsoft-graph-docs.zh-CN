---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 583ac2fe946dc0a987e7495a2862ca17194f6be26dc9bb4d369eb3a94e8315d1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409341"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.connections("contosohr").items("TSP228082938")
    .buildRequest()
    .delete();

```