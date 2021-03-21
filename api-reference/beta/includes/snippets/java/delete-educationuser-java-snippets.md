---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e7a07f09133bc15a912b18bc30e8eea463fc64cc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983180"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().users("13019")
    .buildRequest()
    .delete();

```