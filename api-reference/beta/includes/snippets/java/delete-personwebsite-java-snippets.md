---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea905b452686829a0353c6b7f191a5584af1a41188472ef663dd4cf532fd0bb8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903499"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().websites("{id}")
    .buildRequest()
    .delete();

```