---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 34682a044c829d787ba747247eaf52ff36f0a0b2
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36462091"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Attachment attachment = graphClient.me().events("{id}").attachments("{id}")
    .buildRequest()
    .get();

```