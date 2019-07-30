---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c84468155ff5d61f637e79152e54b2e1a47eae4c
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933829"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Call call = graphClient.app().calls("{id}")
    .buildRequest()
    .get();

```