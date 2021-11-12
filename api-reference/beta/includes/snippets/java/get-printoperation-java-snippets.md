---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85802e35a39c806825dbe41eac05679ec5087a488dd53caa1a864c42a8e7d0b5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277289"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintOperation printOperation = graphClient.print().operations("{id}")
    .buildRequest()
    .get();

```