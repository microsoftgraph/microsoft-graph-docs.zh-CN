---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 231e99baafb6d8afb5d9d3560eeddf74aceb521a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975026"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("ba9a3254-9f18-4209-aeb3-9e42a35b5be4")
    .buildRequest()
    .delete();

```