---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36f2ebf919a7c09452c8eea02da02d931b56ee02
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968793"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.schemaExtensions("{id}")
    .buildRequest()
    .delete();

```