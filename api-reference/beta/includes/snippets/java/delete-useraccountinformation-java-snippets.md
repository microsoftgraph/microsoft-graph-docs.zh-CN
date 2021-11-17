---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e2c6b0d1a88dbe3f65d291524abe5185b9254ce88cccd1efd078c5cb88fed8c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332840"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().account("{id}")
    .buildRequest()
    .delete();

```