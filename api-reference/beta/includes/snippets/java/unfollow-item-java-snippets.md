---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 228c3890adee6bf5c7f308d255268667ec4df6dd
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933806"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{item-id}").unfollow()
    .buildRequest()
    .delete();

```