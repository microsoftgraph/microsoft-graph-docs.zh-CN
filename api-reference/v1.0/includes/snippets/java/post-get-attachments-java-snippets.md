---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 80a36e2a0cbc3dfddca1156538501ad6bdd7b7a1
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36462078"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAttachmentCollectionPage attachments = graphClient.groups("{id}").threads("{id}").posts("{id}").attachments()
    .buildRequest()
    .get();

```