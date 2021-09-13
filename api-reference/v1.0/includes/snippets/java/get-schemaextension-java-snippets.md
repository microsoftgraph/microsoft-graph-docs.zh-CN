---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61e96630c37e9483fde812f081b3ca131f1b72b3b10508b809b88f29a487865b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106996"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SchemaExtension schemaExtension = graphClient.schemaExtensions("graphlearn_test")
    .buildRequest()
    .get();

```