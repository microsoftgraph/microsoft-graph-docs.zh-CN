---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b123f9f371ec6e31e4891592e4fece4502e8b60
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956756"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directory().deletedItems("{object-id}")
    .buildRequest()
    .delete();

```