---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86c4767647d6a2be00e44de3f85ac060934e25ed10f0f5e96cbc7bf15ec3cbbd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105577"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{item-id}")
    .follow()
    .buildRequest()
    .post();

```