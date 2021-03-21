---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d28a615a9d7ac87aaba6fb71ba0801e62ce94230
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977312"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().languages("{id}")
    .buildRequest()
    .delete();

```