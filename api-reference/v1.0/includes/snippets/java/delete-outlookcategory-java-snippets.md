---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20b8ff51c53c0ddcf3e23f1a5cc597db3219d86f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981216"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().outlook().masterCategories("4b1c2495-54c9-4a5e-90a2-0ab0b31987d8")
    .buildRequest()
    .delete();

```