---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99565947d86f41d39bb92ab976a9a37bc7151590
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50966780"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().publications("{id}")
    .buildRequest()
    .delete();

```